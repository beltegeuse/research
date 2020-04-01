+++
title = "Delayed Rejection Metropolis Light Transport"
date = 2020-02-28

[extra]
authors = ["D Rioux-Lavoie*", "J Litalien*", "A Gruson", "T Hachisuka", "D Nowrouzezahrai"]
publication = "*ACM Trans. Graph.* (Accepted), 2020."
join_first = true

image = "drmlt.png"
image_preview = "drmlt_prev.png"

url = [["PDF (preprint)", "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2020_DRMLT.pdf"],
    ["Additional","http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2020_DRMLT/"]]
+++

### Abstract

Designing robust mutation strategies for primary sample space Metropolis light transport is a challenging problem: poorly-tuned mutations both hinder state space exploration and introduce structural image artifacts. Scenes with complex materials, lighting and geometry make hand-designing strategies that remain optimal over the entire state space infeasible. Moreover, these difficult regions are often sparse in state space, and so relying exclusively on intricate (often expensive) proposal mechanisms can be wasteful where simpler inexpensive mechanisms are more sample efficient. We generalize Metropolis--Hastings light transport to employ a flexible two-stage mutation strategy based on delayed rejection  [Green and Mira 2001; Tierneyand Mira 1999]. Our approach generates multiple proposals based on the failure of previous ones, all while preserving Markov chain ergodicity. This allows us to reduce error while maintaining fast global exploration and low correlation across chains. Direct application of delayed rejection to light transport leads to low acceptance  robabilities, and so we also propose a novel transition kernel to alleviate this issue. We benchmark our approach on several applications including _bold-then-timid_ and  _cheap-then-expensive_ proposals across different light transport algorithms. Our method is applicable to any primary sample space algorithm with minimal implementation effort, producing consistently better results on a variety of challenging scenes.