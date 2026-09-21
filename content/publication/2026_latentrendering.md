+++
title = "Physically Based Rendering in the Latent Space"
date = 2026-09-17

[extra]
authors = [
    { name = "Vuk Radovanovic", institution = "Trinity College Dublin"},
    { name = "Vishesh Gupta", institution = "Trinity College Dublin" },
    { name = "Adrien Gruson", institution = "École de Technologie Supérieure" },
    { name = "Binh-Son Hua", institution = "Trinity College Dublin" },
]
join_first = false

publication = "*Computer Graphics Forum (Proceedings of Pacific Graphics)*, 2026."
image = "latent-teaser.png"
image_preview = "latent-thumb.png"
short_description = "Light transport simulation inside the latent space of generative models"

download = [
    { type = "paper", url = "https://arxiv.org/pdf/2609.21054", desc = "pre-peer reviewed version (arXiv)" },
    { type = "doi", url = "https://doi.org/10.1111/cgf.70633" },
    { type = "code", url = "https://github.com/trinity-graphics/latent-rendering" },
    { type = "additional", url = "https://arxiv.org/abs/2609.21054", desc = "arXiv page" },
]

abstract = """Image diffusion models have shown impressive image generation capabilities but are often hard to control, in contrast to classical computer graphics pipelines such as physically based rendering. However, we observe that there is a bridge between light transport phenomena and the distribution of latent space values produced by such models. Thus, we introduce physically based rendering in the feature space learned by the variational autoencoders in generative models, enabling light transport simulation in the latent space. This allows us to leverage physically based rendering techniques to output latent maps for physically guided content generation. We propose modifications to the rendering equation, which, when paired with a differentiable renderer, can yield an optimal set of scene parameters that require only minimal refinement to accurately render into the pretrained latent space. We train our method on a single rendered image, and then demonstrate the generalization of the method to scene geometry changes, lighting changes, and camera view changes."""

bibtex = """@article{Radovanovic:2026:LatentRendering,
    title = {Physically Based Rendering in the Latent Space},
    author = {Vuk Radovanovic and
              Vishesh Gupta and
              Adrien Gruson and
              Binh-Son Hua},
    journal = {Computer Graphics Forum},
    year = {2026},
    doi = {10.1111/cgf.70633}
}
"""

+++

*This is the pre-peer reviewed version of the following article: Radovanovic V., Gupta V., Gruson A., Hua B.-S.: Physically Based Rendering in the Latent Space. Computer Graphics Forum (2026), which will be published in final form at [https://doi.org/10.1111/cgf.70633](https://doi.org/10.1111/cgf.70633). This article may be used for non-commercial purposes in accordance with Wiley Terms and Conditions for Use of Self-Archived Versions.*
