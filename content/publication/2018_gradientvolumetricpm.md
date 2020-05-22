+++
title = "Gradient-domain Volumetric Photon Density Estimation"
date = 2018-04-01

[extra]
authors = [
    { name = "Adrien Gruson", institution = "The University of Tokyo, JFLI, Japan" },
    { name = "Binh-Son Hua", institution = "The University of Tokyo, Japan" },
    { name = "Nicolas Vibert", institution = "McGill University, Canada" },
    { name = "Derek Nowrouzezahrai", institution = "McGill University, Canada" },
    { name = "Toshiya Hachisuka", institution = "The University of Tokyo, Japan" }
]

image = "GradientVolumetricPM.png"
image_preview = "GradientVolumetricPM_prev.png"
publication = "*ACM Trans. Graph. (SIGGRAPH)*, 2018."
short_description = "Gradient-domain formulation of volumetric photon density estimation including beams and planes."

download = [
    { type = "paper", url = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2018_GVPM.pdf"},
    { type = "doi", url = "https://doi.org/10.1145/3197517.3201363" },
    { type = "code", url = "https://github.com/gradientpm/gvpm" },
    { type = "slides", url="http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2018_GVPM/GVPM_Presentation.pptx"},
    { type = "additional", desc = "Web interactive comparison", url="http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2018_GVPM/comparison/index.html"}
]

abstract = """Gradient-domain rendering can improve the convergence of surface-based light transport by exploiting smoothness in image space. Scenes with participating media exhibit similar smoothness and could potentially benefit from gradient-domain techniques. We introduce the first gradient-domain formulation of image synthesis with homogeneous participating media, including four novel and efficient gradient-domain volumetric density estimation algorithms. We show that naive extensions of gradient domain path-space and density estimation methods to volumetric media, while functional, can result in inefficient estimators. Focussing on point-, beam- and plane-based gradient-domain estimators, we introduce a novel shift mapping that eliminates redundancies in the naive formulations using spatial relaxation within the volume. We show that gradient-domain volumetric rendering improve convergence compared to primal domain state-of-the-art, across a suite of scenes. Our formulation and algorithms support progressive estimation and are easy to incorporate atop existing renderers."""

bibtex = """@article{Gruson:2018:GradientVPM,
  title={Gradient-domain volumetric photon density estimation},
  author={Gruson, Adrien and Hua, Binh-Son and Vibert, Nicolas and Nowrouzezahrai, Derek and Hachisuka, Toshiya},
  journal={ACM Transactions on Graphics (TOG)},
  volume={37},
  year={2018},
  doi={10.1145/3197517.3201363}
}"""

+++

