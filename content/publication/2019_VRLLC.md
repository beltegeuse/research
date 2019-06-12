+++
abstract = "Virtual ray lights (VRL) are a powerful representation for multiple-scattered light transport in volumetric participating media. While efficient Monte Carlo estimators can importance sample the contribution of a VRL along an entire sensor subpath, render time still scales linearly in the number of VRLs. We present a new scalable hierarchial VRL method that preferentially samples VRLs according to their image contribution. Similar to Lightcuts-based approaches, we derive a tight upper bound on the potential contribution of a VRL that is efficient to compute. Our bound takes into account the sampling probability densities used when estimating VRL contribution. Ours is the first such upper bound formulation, leading to an efficient and scalable rendering technique with only a few intuitive user parameters. We benchmark our approach in scenes with many VRLs, demonstrating improved scalability compared to existing state-of-the-art techniques."
authors = ["N Vibert", "A Gruson", "H Stokholm", "T Mortensen", "W Jarosz", "T Hachisuka", "D Nowrouzezahrai"]
date = "2019-06-12"
image = "publications/VRLLC.jpg"
image_preview = "publications/VRLLC_prev.jpg"
math = true
publication_types = [2]
publication = "*EGSR* 2019"
publication_short = "*EGSR* 2019"
selected = true
title = "Scalable Virtual Ray Lights Rendering for Participating Media"

#url_code = "#"
#url_pdf = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2018_GVPM.pdf"
#url_project = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2019_GradientSTAR/"
#url_slides = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2018_GVPM/GVPM_Presentation.pptx"
#url_video = "#"

#[[url_custom]]
#name = "HTML Res. + Code"
#url = "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2018_GVPM/comparison/index.html"

+++