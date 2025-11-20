+++
title = "Adaptive Neural Kernels for Gradient-domain Rendering"
date = 2025-12-15

[extra]
authors = [
    { name = "Matthieu Josse", institution = "École Polytechique, Paris"},
    { name = "Joey Litalien", institution = "Independent" },
    { name = "Adrien Gruson", institution = "École de Technologie Supérieure" },
]
join_first = false

publication = "*SIGGRAPH Asia*, 2025."
image = "ank-teaser.png"
image_preview = "ank-thumb.png"
short_description = "Adaptive kernel prediction for gradient-domain rendering"

download = [
    { type = "project", url = "https://mattjosse.github.io/articles/ank/" },
    { type = "code", url = "https://github.com/MattJosse/adaptive-neural-kernel"},
]

abstract = """Monte Carlo methods are a cornerstone of physics-based light transport simulations, valued for their ability to produce high-quality photorealistic images. These stochastic methods often suffer from variance, resulting in undesirable noise in the rendered images. Gradient-domain rendering (GDR) techniques mitigate this problem by estimating unbiased image-space gradients via so-called shift-mapping operators. While these mappings are computationally efficient, they can yield high-variance gradients—and thus poor reconstruction quality—when applied to pixels with wildly different integrals. We tackle this challenge by dynamically selecting the optimal set of neighboring pixels for applying shift-mapping under random sequence replay. Key to our approach is a differentiable sorting network that softly ranks the output of a convolutional neural network conditioned on input sample features for weighted reconstruction. This module is carefully rigidified over time to converge to a hard top-k selection, allowing end-to-end optimization with respect to the reconstruction error. Our method is versatile and can be jointly optimized with other adaptive sampling strategies. We demonstrate variance reduction over other traditional adaptive gradient-domain methods across scenes of varying radiometric complexity."""

bibtex = """@inproceedings{Josse:2025:ANK,
    title = {Adaptive Neural Kernels for Gradient-domain Rendering},
    author = {Matthieu Josse and
              Joey Litalien and
              Adrien Gruson},
    journal = {ACM SIGGRAPH Asia 2025 Conference Proceedings},
    year = {2025},
    month = dec,
    doi = {10.1145/3680528.3687566}
}
"""

+++