# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Adrien Gruson's academic research website, built with [Zola](https://www.getzola.org/) (currently 0.23.6, installed via Homebrew). It is deployed at `https://profs.etsmtl.ca/agruson/`. There is no JS build step, no tests, and no linter — Zola compiles the Sass and templates directly.

Templates use **Tera 2** (Zola 0.23+): macros and `{% import %}` are gone, replaced by globally registered components — `{% component macros.foo(a, b) %}...{% endcomponent macros.foo %}` in `templates/macros.html`, called as `{{ <macros.foo a={expr} b={expr} /> }}` with no import. The `map`, `concat`, `filter` and `slice` filters were also removed; use list comprehensions (`[a.name for a in authors]`), array spread (`[...xs, ...ys]`) and Python-style slicing (`authors[:2]`) instead.

## Commands

```sh
zola serve        # live-reload dev server on http://127.0.0.1:1111
zola build        # render to public/ (gitignored)
zola check        # validate internal + external links
```

`_scripts/publish_toghpages.sh` pushes a build to the `gh-pages` branch, but it hardcodes a `zola` path from an older Linux machine (`/home/agruson/projects/...`). Fix that line before running it, and note it refuses to run on a dirty working tree.

## Architecture

Everything on the site is rendered from **TOML front matter**, not from Markdown bodies. A publication's `.md` body is usually empty; the templates read `page.extra.*`. Adding content means editing front matter (and sometimes `config.toml`), rarely editing templates.

`[slugify] paths = "off"` — the filename *is* the URL segment, so `content/publication/2026_NPPM.md` → `/publication/2026_NPPM/`. Renaming a file breaks external links.

### Publications — `content/publication/*.md`

One file per paper, named `<year>_<ShortName>.md`. Rendered by `templates/publications.html` (the list) and `templates/publication.html` (the detail page). Required `[extra]` keys, as in [2026_NPPM.md](content/publication/2026_NPPM.md):

- `authors` — array of `{ name, institution }`, in paper order.
- `join_first` — `true` marks the first *two* authors as equal contributors (hardcoded to 2 in both templates).
- `publication` — venue string, parsed as inline Markdown (e.g. `"*Eurographics*, 2026."`).
- `image` / `image_preview` — banner and list thumbnail, resolved against `static/publication/`.
- `short_description` — one line shown next to the thumbnail in the list.
- `download` — array of `{ type, url, desc? }`; see **Link rules** below.
- `abstract`, `bibtex` — multiline strings.

`date` drives the ordering (`sort_by = "date"`); future dates are intentional for accepted-but-unpublished papers.

### Link rules

**No paper file is ever committed to this repo** — PDFs, slides, videos and supplemental material are all hosted externally and referenced by URL.

Recognized `download` types: `project`, `paper`, `doi`, `code`, `poster`, `slides`, `video`, `additional`. Only the **first** entry of each type is rendered (except `additional`, which loops). Template behaviour to keep in mind:

- If a `project` entry exists, the list page shows **only** "Project page" and hides every other link — so a paper with a self-hosted project site does not need the rest duplicated here.
- `additional` entries **must** have a `desc`; it is used as the link text. Anything else ignores `desc` except `paper` and `code`, where it is appended after the link.

Where each URL points:

- `paper` — the author's version. **Prefer arXiv**: `https://arxiv.org/pdf/<id>` with `desc = "pre-peer reviewed version (arXiv)"`, and add the abstract page as an `additional` entry (`https://arxiv.org/abs/<id>`, `desc = "arXiv page"`). See [2026_latentrendering.md](content/publication/2026_latentrendering.md). If there is no arXiv version, upload the PDF to the Microsoft cloud storage served at `data.adrien-gruson.com`, under `research/<year>_<ShortName>_<FirstAuthorLastName>.pdf`.
- `doi` — always `https://doi.org/<doi>`; rendered as "Publisher's official version", so never point it at a PDF.
- `code` — the public GitHub/GitLab repository.
- `slides`, `video`, `poster`, `additional` — supplemental files, grouped per paper under `data.adrien-gruson.com/research/<year>_<ShortName>/` (e.g. `.../2020_SMCMC/SMCMC_slides.pptx`, `.../comparison/index.html`).

### Images

Two images per paper, both committed to `static/publication/` and referenced by bare filename:

- `image` — `<name>-teaser.png`: the wide, full-resolution banner shown on the paper's own page.
- `image_preview` — `<name>-thumb.png`: a **square** low-resolution thumbnail (256–512 px) for the publication list.

Older entries use the legacy `<name>.png` / `<name>_prev.png` pair; leave those alone, but use the `-teaser` / `-thumb` naming for anything new.

### Collaborator directory — `config.toml` `[extra].websites`

A flat list of `{ name, url }`. The `macros.one_author_with_link` component (`templates/macros.html`) matches an author's `name` against this list by **exact string equality** and turns it into a link; no match means plain text. So when adding a paper with a new co-author, add them to `websites` with the name spelled identically to the `authors` entry.

Two other things depend on that exact spelling:
- `publications.html` bolds the string `"Adrien Gruson"` via `replace`, so his name must always be written exactly that way.
- The **peer-reviewing conflicts** paragraph on the home page is generated in `templates/index.html` by collecting all author names from publications dated within the last two years, deduplicating, and dropping "Adrien Gruson". It updates itself when a paper is added — do not maintain it by hand.

### Students — `content/students.json`

Loaded by `load_data` in `templates/index.html`. Two arrays, `students` (current) and `graduated` (past), each entry `{ name, type, cosupervised?: [names], remote?: bool }`. `type` must be one of `"Post doc."`, `"Ph.D."`, `"M. Ing"`, `"M.Sc."`, `"Intern"` — any other value silently renders without an icon. Each list is laid out into two columns by interleaving even/odd indices, so order in the JSON is reading order down alternating columns.

`content/students.md` is the separate prospective-students guidelines page (`/students/`), unrelated to this JSON.

### Rendering competition — `content/competition/<year>.md`

`[extra].entries` is an array of `{ name, type, url, image }` where `type` is `winner`, `runnup` (sic), or `entry`. `url` and `image` are paths under `static/competition/<year>/<team>/`, which holds each team's rendered image and report page. Linked from the home page through `config.toml`'s `extra.extrainfo` HTML, not from the navbar.

### Home page and standalone pages

The home page content (biography, job title, interests, education, funding, courses) lives in `config.toml` under `[extra]` — `biography` and `extrainfo` are Markdown/HTML blobs rendered into `templates/index.html`. `templates/index.html` is also the base layout every other template extends, via `{% block content %}` and `{% block scripts %}`.

`content/others.md` (service, talks, older publications) uses the default `templates/page.html`.

### Styling

`compile_sass = true`, so `sass/style.scss` → `style.css` at build time. `sass/academic/` and `sass/vendor/bootstrap/` are ported from the hugo-academic theme. Bootstrap 4 JS, jQuery, Font Awesome and Academicons are loaded from CDNs in `templates/index.html`.
