+++
date = 2018-11-01
title = "Light Transport Simulation in the Gradient Domain"

[extra]
authors = ["B.-S Hua", "A Gruson", "M Zwicker", "T Hachisuka"]

image = "GradientCourse.png"
image_preview = "GradientCourse_prev.png"
math = true
publication_types = [7]
publication = "*SIGGRAPH Asia (Course)*, 2018."
publication_short = "*SIGGRAPH Asia* 2018 Course"
selected = true

url = [["Project page", "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2018_GradientCourse/"],
    ["Additional", "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2018_GVPM/comparison/index.html"]]
+++

### Abstract

Despite the wide adoption in film production and animation industry nowadays, Monte Carlo light transport simulation is still prone to producing noisy images within short rendering time. Accelerating the convergence of Monte Carlo rendering without sacrificing its accuracy is by far a challenging task. In this course, we will learn about gradient-domain light transport simulation, a recent family of techniques in physically based rendering introduced in the past five years that can accelerate traditional Monte Carlo rendering up to approximately an order of magnitude based on gradient estimation and image reconstruction. Particularly, we will introduce the fundamentals of gradient-domain rendering with gradient-domain path tracing, and then extend the discussion to gradient-domain bidirectional path tracing and photon density estimation. We also discuss volume rendering in the gradient domain before diving into advanced topics in recent state-of-the-art papers in this direction. We further discuss tips and tricks in open-source implementations of such algorithms, and provide ideas for future research directions.