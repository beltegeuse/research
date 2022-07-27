+++
title = "Single-pass stratified importance resampling"
date = 2022-06-22

[extra]
authors = [
    { name = "Ege Ciklabakkal", institution = "University of Waterloo, Canada"},
    { name = "Adrien Gruson", institution = "École de Technologie Supérieure" },
    { name = "Iliyan Georgiev", institution = "Autodesk, UK" },
    { name = "Derek Nowrouzezahrai", institution = "McGill University, Canada" },
    { name = "Toshiya Hachisuka", institution = "University of Waterloo, Canada" },
]
join_first = false

publication = "*EGSR*, 2022."
image = "SIS.svg"
image_preview = "SIS_prev.png"
short_description = "Stratification made available within resampled importance sampling"

download = [
    { type = "paper", url = "http://adrien-gruson.com/research/2022_StratifiedResampling/2022_StratifiedResampling.pdf"},
    { type = "doi", url = "https://doi.org/10.1111/cgf.14585" },
    { type ="additional", desc = "Web interactive comparison", url = "http://adrien-gruson.com/research/2022_StratifiedResampling/"},
    { type ="additional", desc = "EGSR 2022 Presentation", url = "http://adrien-gruson.com/research/2022_StratifiedResampling/2022_StratifiedResampling.mp4"},
    #{ type = "code", url = "https://github.com/beltegeuse/rustlight/tree/point-normal"},
    #{ type = "slides", url = "https://adrien-gruson.com/research/2021_PointNormal/volume_product_sampling_EGSR2021.pptx" }
]

abstract = """Resampling is the process of selecting from a set of candidate samples to achieve a distribution (approximately) proportional to a desired target. Recent work has revisited its application to Monte Carlo integration, yielding powerful and practical importance sampling methods. One drawback of existing resampling methods is that they cannot generate stratified samples. We propose two complementary techniques to achieve efficient stratified resampling. We first introduce bidirectional CDF sampling which yields the same result as conventional inverse CDF sampling but in a single pass over the candidates, without needing to store them, similarly to reservoir sampling. We then order the candidates along a space-filling curve to ensure that stratified CDF sampling of candidate indices yields stratified samples in the integration domain. We showcase our method on various resampling-based rendering problems."""

bibtex = """@article{Ciklabakkal:2022:StratifiedResampling,
  author = {Ege Ciklabakkal and Adrien Gruson and Iliyan Georgiev and Derek Nowrouzezahrai and Toshiya Hachisuka},
  title = {Single-pass stratified importance resampling},
  journal = {Computer Graphics Forum (Proceedings of EGSR)},
  year = {2022},
  number = {4},
  volume = {41},
  doi = {10.1111/cgf.14585},
}
"""

+++


