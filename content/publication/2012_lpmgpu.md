+++
date = 2012-02-01
title = "Light Propagation Maps on Parallel Graphics Architectures"

[extra]
authors = [
    { name = "Adrien Gruson", institution = "IRISA, University of Rennes 1, France" },
    { name = "Ajit Hakke Patil", institution = "University of Central Florida, USA" },
    { name = "Remi Cozot", institution = "IRISA, University of Rennes 1, France" },  
    { name = "Kadi Bouatouch", institution = "IRISA, University of Rennes 1, France" },
    { name = "Sumanta Pattanaik", institution = "University of Central Florida, USA" }
]

image = "lpm.png"
image_preview = "lpm_repr.png"
publication = "*EGPVG*, 2012."
short_description = "GPU implementation of light propagation maps."

download = [
    { type = "paper", url = "https://data.adrien-gruson.com/research/2012-LPM-GPU_Gruson.pdf"},
    { type = "doi", url = "http://dx.doi.org/10.2312/EGPGV/EGPGV12/081-088"}
]

abstract = """Light going through a participating medium like smoke can be scattered or absorbed by every point in the medium. To accurately render such a medium we must compute the radiance resulting at every point inside the medium because of these physical effects, which have been modeled by the radiative transfer equation. Computing the radiance at any point inside a participating medium amounts to numerically solving this radiative transport equation. Discrete Ordinate Method (DOM) is a widely used solution method. DOM is computationally intensive. Fattal [Fat09] proposed Light Propagation Maps (LPM) to expedite DOM computation. In this paper we propose a streaming based parallelization of LPM to run on SIMD graphics hardware. Our method is fast and scalable. We report more than 20× speed improvement by using our method as compared to Fattal’s original method. Using our approach we are able to render 64 × 64 × 64 dynamic volumes with multiple scattering of light at interactive speed on complex lighting, and are able to render volumes of any size independent of the GPU memory capability."""

bibtex = """@inproceedings{Gruson:2012:Light,
    title = {Light Propagation Maps on Parallel Graphics Architectures.},
    author = {Gruson, Adrien and Patil, Ajit Hakke and Cozot, R{\\'e}mi and Bouatouch, Kadi and Pattanaik, Sumanta},
    booktitle = {Eurographics Symposium on Parallel Graphics and Visualization},
    publisher = {The Eurographics Association},
    year = {2012},
    doi = {10.2312/EGPGV/EGPGV12/081-088}
}"""

+++

### Video
<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZuEvoZXgOik" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>