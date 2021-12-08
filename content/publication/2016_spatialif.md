+++
date = 2016-08-01
title = "A Spatial Target Function for Metropolis Photon Tracing"

[extra]
abstract_short = "We present a new target function for Metropolis photon tracing that ensures good stratification of photons leading to pixel estimates with equalized relative error. We develop a hierarchical scheme for progressive construction of the target function from paths sampled during rendering."
authors = [
    { name = "Adrien Gruson", institution = "IRISA, University of Rennes 1, France" },
    { name = "Mickael Ribardiere", institution = "XLIM-SIC, University of Poitiers, France" }, 
    { name = "Martin Sik", institution = "Charles University, Czech Republic" },
    { name = "Jiri Vorba", institution = "Charles University, Czech Republic" },
    { name = "Remi Cozot", institution = "IRISA, University of Rennes 1, France" },
    { name = "Kadi Bouatouch", institution = "IRISA, University of Rennes 1, France" },
    { name = "Jaroslav Krivanek", institution = "Charles University, Czech Republic" }
]

image = "spatialTF.png"
image_preview = "spatialTF_prev.png"
publication = "*ACM Trans. Graph,* 2016 (Presented at Siggraph 2017)."
short_description = "Progressive target function to better distribute error in image plane."

download = [
    { type = "paper", url = "https://dl.acm.org/authorize?N23812" },
    { type = "doi", url = "https://doi.org/10.1145/3072959.2963097" },
    { type ="slides", url = "https://adrien-gruson.com/research/2016_SpatialTF/SpatialIF.pptx"},
    { type ="additional", desc="Additional report", url = "https://adrien-gruson.com/research/2016_SpatialTF/supplemental.pdf"},
    { type = "code", url="https://github.com/beltegeuse/spatialTF_code" },
    { type ="additional", desc="Web interactive comparison and scenes", url = "https://adrien-gruson.com/research/2016_SpatialTF/comparison/index.html"}]

abstract = """The human visual system is sensitive to relative differences in luminance but light transport simulation algorithms based on Metropolis sampling often result in a highly non-uniform relative error distribution over the rendered image. While this issue has previously been addressed in the context of the Metropolis light transport algorithm, our work focuses on Metropolis photon tracing. We present a new target function for Metropolis photon tracing that ensures good stratification of photons leading to pixel estimates with equalized relative error. We develop a hierarchical scheme for progressive construction of the target function from paths sampled during rendering. In addition to the approach taken in previous work, where the target function is defined in the image plane, ours can be associated with compact spatial regions. This allows us to take advantage of illumination coherence to more robustly estimate the target function while adapting to geometry discontinuities. To sample from this target function, we design a new replica exchange Metropolis scheme. We apply our algorithm in progressive photon mapping and show that it often outperforms alternative approaches in terms of image quality by a large margin."""

bibtex = """@article{Gruson:2016:SpatialTF,
  title={A spatial target function for metropolis photon tracing},
  author={Gruson, Adrien and Ribardi{\\`e}re, Micka{\\"e}l and {\\v{S}}ik, Martin and Vorba, Ji{\\v{r}}{\\'\\i} and Cozot, R{\\'e}mi and Bouatouch, Kadi and K{\\v{r}}iv{\\'a}nek, Jaroslav},
  journal={ACM Transactions on Graphics (TOG)},
  volume={36},
  year={2016},
  doi={10.1145/3072959.2963097}
}"""

+++