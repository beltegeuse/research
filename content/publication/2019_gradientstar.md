+++
title = "A Survey on Gradient-Domain Rendering"
date = 2019-03-12

[extra]
authors = ["B.-S Hua", "A Gruson", "V Petitjean", "M Zwicker", "D Nowrouzezahrai", "E Eisemann", "T Hachisuka"]

image = "gradientdomain_star.jpg"
image_preview = "gradientdomain_star_prev.png"

publication = "*Eurographics (STAR)*, 2019."

url = [["Project page", "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2019_GradientSTAR/"]]
+++

### Abstract

Monte Carlo methods for physically-based light transport simulation are broadly adopted in film productions and animation/visual effects industries. Monte Carlo methods, however, often result in noisy images and have slow convergence. As such, improving the convergence of Monte Carlo rendering remains an important open problem. Gradient-domain light transport is a recent family of techniques that can accelerate Monte Carlo rendering by up to an order of magnitude, leveraging a gradient-based estimation and a reformulation of the rendering problem as an image reconstruction. This state of the art report comprehensively elaborates the fundamentals of gradient-domain rendering, as well as the specifics behind gradient-domain uni- and bidirectional path tracing and gradient-domain photon density estimation. We also discuss various image reconstruction schemes which are important components of gradient-domain rendering. Finally, we benchmark various gradient-domain techniques against state-of-the-art denoising methods before discussing open problems.