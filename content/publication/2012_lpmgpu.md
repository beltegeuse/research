+++
date = 2012-02-01
title = "Light Propagation Maps on Parallel Graphics Architectures"

[extra]
authors = ["A Gruson", "A Hakke Patil", "R Cozot", "K Bouatouch", "S Pattanaik"]
image = "lpm.png"
image_preview = "lpm_repr.png"
math = true
publication_types = ["2"]
publication = "*EGPVG*, 2012."
selected = false
url = [["PDF", "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2012-LPM-GPU_Gruson.pdf"]]

+++

### Abstract

Light going through a participating medium like smoke can be scattered or absorbed by every point in the medium. To accurately render such a medium we must compute the radiance resulting at every point inside the medium because of these physical effects, which have been modeled by the radiative transfer equation. Computing the radiance at any point inside a participating medium amounts to numerically solving this radiative transport equation. Discrete Ordinate Method (DOM) is a widely used solution method. DOM is computationally intensive. Fattal [Fat09] proposed Light Propagation Maps (LPM) to expedite DOM computation. In this paper we propose a streaming based parallelization of LPM to run on SIMD graphics hardware. Our method is fast and scalable. We report more than 20× speed improvement by using our method as compared to Fattal’s original method. Using our approach we are able to render 64 × 64 × 64 dynamic volumes with multiple scattering of light at interactive speed on complex lighting, and are able to render volumes of any size independent of the GPU memory capability.

### Video
<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZuEvoZXgOik" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>