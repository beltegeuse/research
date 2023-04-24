+++
title = "Regression-based Monte Carlo Integration"
date = 2022-06-15

[extra]
authors = [
    { name = "Corentin Salaun", institution = "Max-Planck-Institut fur Informatik, Germany"},
    { name = "Adrien Gruson", institution = "McGill University & École de Technologie Supérieure" },
    { name = "Binh-Son Hua", institution = "VinAI Research, Vietnam" },
    { name = "Toshiya Hachisuka", institution = "University of Waterloo, Canada" },
    { name = "Gurprit Singh", institution = "Max-Planck-Institut fur Informatik, Germany"}
]
join_first = false

publication = "*ACM Trans. Graph.* (SIGGRAPH), 2022."
image = "regressionMC.jpg"
image_preview = "regressionMC_prev.png"
short_description = "Probably more efficient MC estimator based on regression"

download = [
    { type = "paper", url = "https://data.adrien-gruson.com/research/2022_RegressionMC_Salaun.pdf"},
    { type = "doi", url = "https://doi.org/10.1145/3528223.3530095" },
    { type ="additional", desc = "Web interactive comparison", url = "https://data.adrien-gruson.com/research/2022_RegressionMC/index.html"},
    { type = "code", url = "https://github.com/iribis/regressionmc"},
]

abstract = """Monte Carlo integration is typically interpreted as an estimator of the expected value using stochastic samples. There exists an alternative interpretation in calculus where Monte Carlo integration can be seen as estimating a *constant* function -- from the stochastic evaluations of the integrand -- that integrates to the original integral. The integral mean value theorem states that this *constant* function should be the mean (or expectation) of the integrand. Since both interpretations result in the same estimator, little attention has been devoted to the calculus-oriented interpretation. We show that the calculus-oriented interpretation actually implies the possibility of using a more *complex* function than a *constant* one to construct a more efficient estimator for Monte Carlo integration. We build a new estimator based on this interpretation and relate our estimator to control variates with least-squares regression on the stochastic samples of the integrand. Unlike prior work, our resulting estimator is *provably* better than or equal to the conventional Monte Carlo estimator. To demonstrate the strength of our approach, we introduce a practical estimator that can act as a simple drop-in replacement for conventional Monte Carlo integration. We experimentally validate our framework on various light transport integrals."""

bibtex = """@article{Salaun:2022:RegressionMC,
    author = {Sala\"{u}n, Corentin and Gruson, Adrien and Hua, Binh-Son and Hachisuka, Toshiya and Singh, Gurprit},
    title = {Regression-Based Monte Carlo Integration},
    year = {2022},
    volume = {41},
    number = {4},
    doi = {10.1145/3528223.3530095},
    journal = {ACM Trans. Graph.},
}"""

+++

#### Presentation

<iframe width="650" height="365" src="https://www.youtube.com/embed/CWVn3L_JghM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

