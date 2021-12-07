+++
title = "Gradient-Domain Photon Density Estimation"
date = 2017-04-01

[extra]
authors = [
    { name = "Binh-Son Hua", institution = "The University of Tokyo, Japan" },
    { name = "Adrien Gruson", institution = "The University of Tokyo, Japan" },
    { name = "Derek Nowrouzezahrai", institution = "McGill University, Canada" },
    { name = "Toshiya Hachisuka", institution = "The University of Tokyo, Japan" }
]

image = "GradientPM.png"
image_preview = "GradientPM_prev.png"
publication = "*Eurographics*, 2017."
short_description = "Gradient-domain formulation of photon density estimation."

download = [
    { type = "paper", url = "https://profs.etsmtl.ca/agruson/DATA/2017_GradientPM_Hua.pdf"},
    { type = "doi", url = "https://doi.org/10.1111/cgf.13104" },
    { type = "code", url = "https://github.com/gradientpm/gpm" },
    { type = "slides", url = "https://profs.etsmtl.ca/agruson/DATA/2017_GPM/presentation_GPM.pptx"},
    { type = "additional", desc = "Web interactive comparison and scenes", url = "https://profs.etsmtl.ca/agruson/DATA/2017_GPM/comparison/index.html"}
]

abstract = """The most common solutions to the light transport problem rely on either Monte Carlo (MC) integration or density estimation methods, such as uni- & bi-directional path tracing or photon mapping. Recent gradient-domain extensions of MC approaches show great promise; here, gradients of the final image are estimated numerically (instead of the image intensities themselves) with coherent paths generated from a deterministic shift mapping. We extend gradient-domain approaches to light transport simulation based on density estimation. As with previous gradient-domain methods, we detail important considerations that arise when moving from a primal- to gradient-domain estimator. We provide an efficient and straightforward solution to these problems. Our solution supports stochastic progressive density estimation, so it is robust to complex transport effects. We show that gradient-domain photon density estimation converges faster than its primal-domain counterpart, as well as being generally more robust than gradient-domain uni- & bi-directional path tracing for scenes dominated by complex transport."""

bibtex = """@inproceedings{Hua:2017:GradientPM,
  title={Gradient-Domain Photon Density Estimation},
  author={Hua, Binh-Son and Gruson, Adrien and Nowrouzezahrai, Derek and Hachisuka, Toshiya},
  booktitle={Computer Graphics Forum},
  volume={36},
  year={2017},
  doi={10.1111/cgf.13104}
}"""

+++

