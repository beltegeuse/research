+++
title = "Practical Product Path Guiding Using Linearly Transformed Cosines"
date = 2020-06-15

[extra]
authors = [
    { name = "Stavros Diolatzis", institution = "Université Côté d’Azur, Inria, France"},
    { name = "Adrien Gruson", institution = "McGill University, Canada" },
    { name = "Wenzel Jackob", institution = "EPFL, Swissland" },
    { name = "Derek Nowrouzezahrai", institution = "McGill University, Canada" },
    { name = "George Drettakis", institution = "Université Côté d’Azur, Inria, France" },
]

publication = "*EGSR*, 2020."
image = "pppg.jpg"
image_preview = "pppg_prev.png"
short_description = "Efficient combinaison of Practical Path guiding and LTC"

download = [
    { type = "paper", url = "http://www-sop.inria.fr/reves/Basilic/2020/DGJND20/practical_product_path_guiding_authors.pdf"},
    { type = "doi", url = "https://diglib.eg.org/handle/10.1111/cgf14051" },
    { type = "additional", desc = "Web interactive comparison", url = "https://repo-sam.inria.fr/fungraph/practical_product_path_guiding/"},
    { type = "code", url = "https://gitlab.inria.fr/sdiolatz/practical-product-path-guiding"},
]

abstract = """Path tracing is now the standard method used to generate realistic imagery in many domains, e.g., film, special effects, architecture etc. Path guiding has recently emerged as a powerful strategy to counter the notoriously long computation times required to render such images. We present a practical path guiding algorithm that performs product sampling, i.e., samples proportional to the product of the bidirectional scattering distribution function (BSDF) and incoming radiance. We use a spatial-directional subdivision to represent incoming radiance, and introduce the use of Linearly Transformed Cosines (LTCs) to represent the BSDF during path guiding, thus enabling efficient product sampling. Despite the computational efficiency of LTCs, several optimizations are needed to make our method cost effective. In particular, we show how we can use vectorization, precomputation, as well as strategies to optimize multiple importance sampling and Russian roulette to improve performance. We evaluate our method on several scenes, demonstrating consistent improvement in efficiency compared to previous work, especially in scenes with significant glossy inter-reflection."""

bibtex = """@article {DGJND20,
  author       = "Diolatzis, Stavros and Gruson, Adrien and Jakob, Wenzel and Nowrouzezahrai, Derek and Drettakis, George",
  title        = "Practical Product Path Guiding Using Linearly Transformed Cosines",
  journal      = "Computer Graphics Forum (Proceedings of the Eurographics Symposium on Rendering)",
  year         = "2020",
  url          = "http://www-sop.inria.fr/reves/Basilic/2020/DGJND20",
  ISSN         = {1467-8659},
  DOI          = {10.1111/cgf.14051}
}"""

+++
