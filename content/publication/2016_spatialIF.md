+++
abstract = "The human visual system is sensitive to relative differences in luminance but light transport simulation algorithms based on Metropolis sampling often result in a highly non-uniform relative error distribution over the rendered image. While this issue has previously been addressed in the context of the Metropolis light transport algorithm, our work focuses on Metropolis photon tracing. We present a new target function for Metropolis photon tracing that ensures good stratification of photons leading to pixel estimates with equalized relative error. We develop a hierarchical scheme for progressive construction of the target function from paths sampled during rendering. In addition to the approach taken in previous work, where the target function is defined in the image plane, ours can be associated with compact spatial regions. This allows us to take advantage of illumination coherence to more robustly estimate the target function while adapting to geometry discontinuities. To sample from this target function, we design a new replica exchange Metropolis scheme. We apply our algorithm in progressive photon mapping and show that it often outperforms alternative approaches in terms of image quality by a large margin."
abstract_short = "We present a new target function for Metropolis photon tracing that ensures good stratification of photons leading to pixel estimates with equalized relative error. We develop a hierarchical scheme for progressive construction of the target function from paths sampled during rendering."
authors = ["A Gruson", "M Ribardiere", "M Sik", "J Vorba", "R Cozot", "K Bouatouch", "J Krivanek"]
date = "2016-08-01"
image = "publications/spatialTF.png"
image_preview = "publications/spatialTF_prev.png"
math = true
publication_types = ["2"]
publication = "In *ACM Transaction on Graphics*, 2016 (Presented at Siggraph 2017)"
publication_short = "In *ACM Trans. Graph.*, 2016 (Presented at Siggraph 2017)"
selected = true
title = "A Spatial Target Function for Metropolis Photon Tracing"
#url_code = "#"
#url_dataset = "#"
#url_pdf = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2016_Spatial-Target-Function_Gruson.pdf"
url_pdf = "https://dl.acm.org/authorize?N23812"
#url_project = "http://people.irisa.fr/Matis.Hudon/Shape.html"
url_slides = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2016_SpatialTF/SpatialIF.pptx"
#url_video = "#"

[[url_custom]]
name = "Additional Mat."
url = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2016_SpatialTF/supplemental.pdf"

[[url_custom]]
name = "HTML Res. + Code"
url = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2016_SpatialTF/comparison/index.html"

+++
