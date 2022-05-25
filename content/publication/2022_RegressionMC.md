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

publication = "ACM Trans. Graph. (SIGGRAPH) 2022."
image = "regressionMC.jpg"
image_preview = "regressionMC_prev.png"
short_description = "Probably more efficient MC estimator based on regression"

download = [
    { type = "paper", url = "https://adrien-gruson.com/research/2022_RegressionMC_Salaun.pdf"},
    #{ type = "doi", url = "https://doi.org/10.2312/sr.20211290" },
    #{ type ="additional", desc="Additional report", url = "https://adrien-gruson.com/research/2021_PointNormal/2021_PointNormal_Villeneuve_additional.pdf"},
    #{ type = "code", url = "https://github.com/beltegeuse/rustlight/tree/point-normal"},
    #{ type = "slides", url = "https://adrien-gruson.com/research/2021_PointNormal/volume_product_sampling_EGSR2021.pptx" }
]

abstract = """Monte Carlo integration is typically interpreted as an estimator of the expected value using stochastic samples. There exists an alternative interpretation in calculus where Monte Carlo integration can be seen as estimating a *constant* function -- from the stochastic evaluations of the integrand -- that integrates to the original integral. The integral mean value theorem states that this *constant* function should be the mean (or expectation) of the integrand. Since both interpretations result in the same estimator, little attention has been devoted to the calculus-oriented interpretation. We show that the calculus-oriented interpretation actually implies the possibility of using a more *complex* function than a *constant* one to construct a more efficient estimator for Monte Carlo integration. We build a new estimator based on this interpretation and relate our estimator to control variates with least-squares regression on the stochastic samples of the integrand. Unlike prior work, our resulting estimator is *provably* better than or equal to the conventional Monte Carlo estimator. To demonstrate the strength of our approach, we introduce a practical estimator that can act as a simple drop-in replacement for conventional Monte Carlo integration. We experimentally validate our framework on various light transport integrals."""

bibtex = """"""

+++

