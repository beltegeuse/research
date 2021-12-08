+++
title = "An Efficient Transport Estimator for Complex Layered Materials"
date = 2020-02-16

[extra]
authors = [
    { name = "Luis Gamboa", institution = "University of Montreal, Canada" },
    { name = "Adrien Gruson", institution = "McGill University, Canada" }, 
    { name = "Derek Nowrouzezahrai", institution = "McGill University, Canada" }
]

publication = "*Eurographics*, 2020."
image = "layered.jpg"
image_preview = "layered_prev.jpg"
short_description = "More efficient estimator for complex layered appearance models."

download = [
    { type = "project", url = "https://lc.fie.umich.mx/~legg/complexlayered.php" },
    { type = "paper", url = "https://adrien-gruson.com/research/2020_EfficientLayered.pdf" },
    { type = "slides", url = "https://adrien-gruson.com/research/2020_Layered/layered_slides.pptx" },
    { type = "video", url = "https://adrien-gruson.com/research/2020_Layered/layered_video.mp4" },
    { type = "doi", url = "https://diglib.eg.org/handle/10.1111/cgf13936" },
    { type = "code", url="https://github.com/leggcg/EfficientComplexLayered" }
]

abstract = """Layered materials capture subtle, realistic reflection behaviors that traditional single-layer models lack. Much of this is due to the complex subsurface light transport at the interfaces of -- and in the media between -- layers. Rendering with these materials can be costly, since we must simulate these transport effects _at every evaluation_ of the underlying reflectance model. Rendering an image requires thousands of such evaluations, _per pixel_. Recent work treats this complexity by introducing significant approximations, requiring large precomputed datasets per material, or simplifying the light transport simulations within the materials. Even the most effective of these methods struggle with the complexity induced by high-frequency variation in reflectance parameters and micro-surface normal variation, as well as anisotropic volumetric scattering between the layer interfaces. We present a more efficient, unbiased estimator for light transport in such general, complex layered appearance models. By conducting an analysis of the types of transport paths that contribute most to the aggregate reflectance dynamics, we propose an effective and unbiased path sampling method that reduces variance in the reflectance evaluations. Our method additionally supports reflectance importance sampling, does not rely on any precomputation, and so integrates readily into existing renderers. We consistently outperform the state-of-the-art by ~2-6x in equal-quality (i.e., equal error) comparisons."""

bibtex = """@article {Gamboa:2020:EfficientLayered,
    journal = {Computer Graphics Forum},
    title = {{An Efficient Transport Estimator for Complex Layered Materials}},
    author = {Gamboa, Luis E. and Gruson, Adrien and Nowrouzezahrai, Derek},
    year = {2020},
    publisher = {The Eurographics Association and John Wiley & Sons Ltd.},
    ISSN = {1467-8659},
    DOI = {10.1111/cgf.13936}
}"""

+++

