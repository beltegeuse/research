+++
title = "Stratified Markov Chain Monte Carlo Light Transport"
date = 2020-02-17

[extra]
authors = [
    { name = "Adrien Gruson", institution = "McGill University, Canada" },
    { name = "Rex West", institution = "The University of Tokyo, Japan" },
    { name = "Toshiya Hachisuka", institution = "The University of Tokyo, Japan" },
]

publication = "*Eurographics*, 2020."
image = "smcmc.jpg"
image_preview = "smcmc_prev.jpg"
short_description = "Perfect image-space stratification with MCMC."

download = [
    { type = "paper", url = "https://profs.etsmtl.ca/agruson/DATA/2020_SMCMC.pdf"},
    { type = "doi", url = "https://diglib.eg.org/handle/10.1111/cgf13935"}, 
    { type = "additional", desc = "Web interactive comparison", url = "https://profs.etsmtl.ca/agruson/DATA/2020_SMCMC/"}, 
    { type = "code", url = "https://github.com/beltegeuse/smcmc"},
    { type = "slides", url = "https://profs.etsmtl.ca/agruson/DATA/2020_SMCMC/SMCMC_slides.pptx" }
]

abstract = """Markov chain Monte Carlo (MCMC) sampling is a powerful approach to generate samples from an arbitrary distribution. The application to light transport simulation allows us to efficiently handle complex light transport such as highly occluded scenes. Since light transport paths in MCMC methods are sampled according to the path contributions over the sampling domain covering the whole image, bright pixels receive more samples than dark pixels to represent differences in the brightness. This variation in the number of samples per pixel is a fundamental property of MCMC methods. This property often leads to uneven convergence over the image, which is a notorious and fundamental issue of any MCMC method to date. We present a novel stratification method of MCMC light transport methods. Our stratification method, for the first time, breaks the fundamental limitation that the number of samples per pixel is uncontrollable. Our method guarantees that every pixel receives a specified number of samples by running a single Markov chain per pixel. We rely on the fact that different MCMC processes should converge to the same result when the sampling domain and the integrand are the same. We thus subdivide an image into multiple overlapping tiles associated with each pixel, run an independent MCMC process in each of them, and then align all of the tiles such that overlapping regions match. This can be formulated as an optimization problem similar to the reconstruction step for gradient-domain rendering. Further, our method can exploit the coherency of integrands among neighboring pixels via coherent Markov chains and replica exchange. Images rendered with our method exhibit much more predictable convergence compared to existing MCMC methods."""

bibtex = """@article {Gruson:2020:SMCMC,
    journal = {Computer Graphics Forum},
    title = {{Stratified Markov Chain Monte Carlo Light Transport}},
    author = {Gruson, Adrien and West, Rex and Hachisuka, Toshiya},
    year = {2020},
    publisher = {The Eurographics Association and John Wiley & Sons Ltd.},
    ISSN = {1467-8659},
    DOI = {10.1111/cgf.13935}
}"""

+++
