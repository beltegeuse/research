+++
title = "Delayed Rejection Metropolis Light Transport"
date = 2020-02-28

[extra]
authors = [
    { name = "Damien Rioux-Lavoie", institution = "McGill University, Canada" },
    { name = "Joey Litalien", institution = "McGill University, Canada" },
    { name = "Adrien Gruson", institution = "McGill University, Canada" },
    { name = "Toshiya Hachisuka", institution = "The University of Tokyo, Japan" },
    { name = "Derek Nowrouzezahrai", institution = "McGill University, Canada" },
]
join_first = true

publication = "*ACM Trans. Graph.*, 2020. (Presented at SIGGRAPH 2020)."
image = "drmlt.png"
image_preview = "drmlt_prev.png"
short_description = "Delayed rejection in MCMC applied to rendering."

download = [
    { type = "paper", url = "https://data.adrien-gruson.com/research/2020_DRMLT.pdf"},
    { type = "doi", url = "https://doi.org/10.1145/3388538"},
    { type = "code", url = "https://github.com/joeylitalien/drmlt" },
    { type = "additional", desc = "Web interactive comparison", url = "https://data.adrien-gruson.com/research/2020_DRMLT/index.html"}
]

abstract = """Designing robust mutation strategies for primary sample space Metropolis light transport is a challenging problem: poorly-tuned mutations both hinder state space exploration and introduce structural image artifacts. Scenes with complex materials, lighting and geometry make hand-designing strategies that remain optimal over the entire state space infeasible. Moreover, these difficult regions are often sparse in state space, and so relying exclusively on intricate (often expensive) proposal mechanisms can be wasteful where simpler inexpensive mechanisms are more sample efficient. We generalize Metropolis--Hastings light transport to employ a flexible two-stage mutation strategy based on delayed rejection  [Green and Mira 2001; Tierneyand Mira 1999]. Our approach generates multiple proposals based on the failure of previous ones, all while preserving Markov chain ergodicity. This allows us to reduce error while maintaining fast global exploration and low correlation across chains. Direct application of delayed rejection to light transport leads to low acceptance  robabilities, and so we also propose a novel transition kernel to alleviate this issue. We benchmark our approach on several applications including _bold-then-timid_ and  _cheap-then-expensive_ proposals across different light transport algorithms. Our method is applicable to any primary sample space algorithm with minimal implementation effort, producing consistently better results on a variety of challenging scenes."""

bibtex = """@article{Rioux-Lavoie:2020:DRMLT,
    author = {Rioux-Lavoie, Damien and Litalien, Joey and Gruson, Adrien and Hachisuka, Toshiya and Nowrouzezahrai, Derek},
    title = {Delayed Rejection {Metropolis} Light Transport},
    journal = {ACM Transactions on Graphics},
    volume = {39},
    number = {3},
    year = {2020},
    month = apr,
    doi = {10.1145/3388538},
}"""

+++

### Presentation 

<iframe width="650" height="365" src="https://www.youtube.com/embed/m22d-cTcubc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>