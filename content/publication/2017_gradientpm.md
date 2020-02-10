+++
title = "Gradient-Domain Photon Density Estimation"
date = 2017-04-01

[extra]
authors = ["B.-S Hua", "A Gruson", "D Nowrouzezahrai", "T Hachisuka"]
image = "GradientPM.png"
image_preview = "GradientPM_prev.png"
math = true
publication_types = ["2"]
publication = "*Eurographics*, 2017."
selected = true

url = [["PDF", "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2017_GradientPM_Hua.pdf"],
    ["Slides","http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2017_GPM/presentation_GPM.pptx"],
    ["Additional", "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2017_GPM/comparison/index.html"]]

+++

### Abstract

The most common solutions to the light transport problem rely on either Monte Carlo (MC) integration or density estimation methods, such as uni- & bi-directional path tracing or photon mapping. Recent gradient-domain extensions of MC approaches show great promise; here, gradients of the final image are estimated numerically (instead of the image intensities themselves) with coherent paths generated from a deterministic shift mapping. We extend gradient-domain approaches to light transport simulation based on density estimation. As with previous gradient-domain methods, we detail important considerations that arise when moving from a primal- to gradient-domain estimator. We provide an efficient and straightforward solution to these problems. Our solution supports stochastic progressive density estimation, so it is robust to complex transport effects. We show that gradient-domain photon density estimation converges faster than its primal-domain counterpart, as well as being generally more robust than gradient-domain uni- & bi-directional path tracing for scenes dominated by complex transport.
