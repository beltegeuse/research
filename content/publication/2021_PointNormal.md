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

publication = "*EGSR* - Digital Library Only Track, 2020."
image = "point_normal.png"
image_preview = "point_normal_prev.png"
short_description = "Different sampling routines for single scattering"

download = [
    { type = "paper", url = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2021_PointNormal_Villeneuve.pdf"},
    #{ type = "doi", url = "#" },
    { type ="additional", desc="Additional report", url = "#"},
    { type = "code", url = "https://github.com/beltegeuse/rustlight/tree/point-normal"},
]

abstract = """Efficient Monte-Carlo estimation of volumetric single scattering remains challenging due to various sources of variance, including transmittance, phase-function anisotropy, geometric cosine foreshortening, and squared-distance fall-off. We propose several complementary techniques to importance sample each of these terms and their product. First, we introduce an extension to equi-angular sampling to analytically account for the foreshortening at point-normal emitters. We then include transmittance and phase function via Taylor-series expansion and/or warp composition. Scaling to complex mesh emitters is achieved through an adaptive tree-splitting scheme. We show improved performance over state-of-the-art baselines in a diversity of scenarios."""

bibtex = """@article{Villeneuve:2021:VolumeProductSampling,
  author = {Keven Villeneuve and Adrien Gruson and Iliyan Georgiev and Derek Nowrouzezahrai},
  title = {Practical product sampling for single scattering in media},
  booktitle = {Proceedings of EGSR - Digital Library Only Track},
  year = {2021},
  month = jun,
  publisher = {The Eurographics Association}
}"""

+++