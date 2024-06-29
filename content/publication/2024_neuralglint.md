+++
title = "Neural Histogram-Based Glint Rendering of Surfaces With Spatially Varying Roughness"
date = 2024-06-22

[extra]
authors = [
    { name = "Ishaan Shah", institution = "CVIT, International Institute of Information Technology, Hyderabad (IIIT-H), India"},
    { name = "Luis Gamboa", institution = "Universidad Michoacana de San Nicolás de Hidalgo, Mexico" },
    { name = "Adrien Gruson", institution = "École de Technologie Supérieure" },
    { name = "P. J. Narayanan", institution = "CVIT, International Institute of Information Technology, Hyderabad (IIIT-H), India" },
]
join_first = false

publication = "*EGSR*, 2024."
image = "neural_glint.png"
image_preview = "neural_glint_prev.png"
short_description = "Appearance filtering and analytical lighting integration of a glinty surface"

download = [
    { type = "project", url = "https://ishaanshah.xyz/neural_glint/" },
    { type = "paper", url = "https://data.adrien-gruson.com/research/2024_NeuralGlint_Shah.pdf"},
    { type = "code", url = "https://github.com/ishaanshah/neural_glint"},
]

abstract = """The complex, glinty appearance of detailed normal-mapped surfaces at different scales requires expensive per-pixel Normal Distribution Function computations. Moreover, large light sources further compound this integration and increase the noise in the Monte Carlo renderer. Specialized rendering techniques that explicitly express the underlying normal distribution have been developed to improve performance for glinty surfaces controlled by a fixed material roughness. We present a new method that supports spatially varying roughness based on a neural histogram that computes per-pixel NDFs with arbitrary positions and sizes. Our representation is both memory and compute efficient. Additionally, we fully integrate direct illumination for all light directions in constant time. Our approach decouples roughness and normal distribution, allowing the live editing of the spatially varying roughness of complex normal-mapped objects. We demonstrate that our approach improves on previous work by achieving smaller footprints while offering GPU-friendly computation and compact representation."""

bibtex = """@article{Shah:2024:NeuralGlint,
  author = {Ishaan Shah and Luis E. Gamboa and Adrien Gruson and P.J. Narayanan},
  title = {Neural Histogram-Based Glint Rendering of Surfaces With Spatially Varying Roughness},
  journal = {Computer Graphics Forum (Proceedings of EGSR)},
  year = {2024},
  number = {4},
  volume = {43},
}
"""

+++

#### Results

Please visit the project website for the video and image viewer: https://ishaanshah.xyz/neural_glint/ 