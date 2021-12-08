+++
title = "Practical product sampling for single scattering in media"
date = 2021-06-15

[extra]
authors = [
    { name = "Keven Villeneuve", institution = "SEED -- Electronic Arts, Canada"},
    { name = "Adrien Gruson", institution = "McGill University, Canada" },
    { name = "Iliyan Georgiev", institution = "Autodesk, United Kingdom" }, 
    { name = "Derek Nowrouzezahrai", institution = "McGill University, Canada" },
]
join_first = true

publication = "*EGSR* - Digital Library Only Track, 2021."
image = "point_normal.png"
image_preview = "point_normal_prev.png"
short_description = "Different sampling routines for single scattering"

download = [
    { type = "paper", url = "https://adrien-gruson.com/research/2021_PointNormal_Villeneuve.pdf"},
    { type = "doi", url = "https://doi.org/10.2312/sr.20211290" },
    { type ="additional", desc="Additional report", url = "https://adrien-gruson.com/research/2021_PointNormal/2021_PointNormal_Villeneuve_additional.pdf"},
    { type = "code", url = "https://github.com/beltegeuse/rustlight/tree/point-normal"},
    { type = "slides", url = "https://adrien-gruson.com/research/2021_PointNormal/volume_product_sampling_EGSR2021.pptx" }
]

abstract = """Efficient Monte-Carlo estimation of volumetric single scattering remains challenging due to various sources of variance, including transmittance, phase-function anisotropy, geometric cosine foreshortening, and squared-distance fall-off. We propose several complementary techniques to importance sample each of these terms and their product. First, we introduce an extension to equi-angular sampling to analytically account for the foreshortening at point-normal emitters. We then include transmittance and phase function via Taylor-series expansion and/or warp composition. Scaling to complex mesh emitters is achieved through an adaptive tree-splitting scheme. We show improved performance over state-of-the-art baselines in a diversity of scenarios."""

bibtex = """@article{Villeneuve:2021:VolumeProductSampling,
  author = {Keven Villeneuve and Adrien Gruson and Iliyan Georgiev and Derek Nowrouzezahrai},
  title = {Practical product sampling for single scattering in media},
  booktitle = {Proceedings of EGSR - Digital Library Only Track},
  year = {2021},
  month = jun,
  publisher = {The Eurographics Association},
  DOI = {10.2312/sr.20211290}
}"""

+++

### Presentation 

<iframe width="650" height="365"src="https://www.youtube.com/embed/iETDEkcRI8M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
