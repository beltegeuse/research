+++
title = "Efficient Energy-Compensated VPLs using Photon Splatting"
date = 2018-03-01

[extra]
authors = ["J Sriwasansak", "A Gruson", "T Hachisuka"]

image = "efficientVPL.png"
image_preview = "efficientVPL_prev.png"
math = true
publication_types = [2]
publication = "*I3D*, 2018."
selected = true

url = [["Project page", "http://jamorn.me/evplp/"],
    ["Code","https://github.com/zentojamorn/evplp"]]

+++

### Abstract

Efficient light transport simulation is important for many applications in computer graphics. Many-light methods based on virtual point lights (VPLs) especially work well for scenes consist mainly of diffuse materials. Rendered images with VPLs, however, are known to suffer from energy loss due to clamping of the VPL contributions. Removing this clamping unfortunately introduces significant variance in images due to the singularities of VPLs. We propose an efficient and practical algorithm which compensates energy loss of VPLs using yet another efficient rendering method -- photon splatting. Recent unified path sampling frameworks shows that VPLs are in fact photons. Based on this unified formulation, we propose to reuse VPLs as photons to compensate missing energy of clamped VPLs. This combination is very natural: the singularities of VPLs happen if a shading point is too close to VPLs, but such VPLs can also be seen as neighboring photons that are indeed useful for photon density estimation. We formulate this energy compensation process using multiple importance sampling to optimally combine rendering with VPLs and photon splatting. Our algorithm can be efficiently implemented on GPUs since rendering with VPLs and photon splatting are both suitable for GPUs. The results demonstrate that our method produces more accurate images in the same rendering time than the existing methods. For common use cases of rendering mostly diffuse scenes, our work leads to an efficient, accurate, and practical rendering algorithm based on VPLs.