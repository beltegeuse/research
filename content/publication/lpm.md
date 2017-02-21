+++
abstract = "Light going through a participating medium like smoke can be scattered or absorbed by every point in the medium. To accurately render such a medium we must compute the radiance resulting at every point inside the medium because of these physical effects, which have been modeled by the radiative transfer equation. Computing the radiance at any point inside a participating medium amounts to numerically solving this radiative transport equation. Discrete Ordinate Method (DOM) is a widely used solution method. DOM is computationally intensive. Fattal [Fat09] proposed Light Propagation Maps (LPM) to expedite DOM computation. In this paper we propose a streaming based parallelization of LPM to run on SIMD graphics hardware. Our method is fast and scalable. We report more than 20× speed improvement by using our method as compared to Fattal’s original method. Using our approach we are able to render 64 × 64 × 64 dynamic volumes with multiple scattering of light at interactive speed on complex lighting, and are able to render volumes of any size independent of the GPU memory capability."
authors = ["A Gruson", "A Hakke Patil", "R Cozot", "K Bouatouch", "S Pattanaik"]
date = "2012-02-01"
image = "publications/lpm.png"
image_preview = ""
math = true
publication_types = ["2"]
publication = "In *Eurographics Symposium on Parallel Graphics and Visualization*, 2012."
publication_short = "In *EGPVG 2012*"
selected = false
title = "Light Propagation Maps on Parallel Graphics Architectures"
#url_code = "#"
#url_dataset = "#"
url_pdf = "projects/lpm_EGPVG2012.pdf"
#url_project = "http://people.irisa.fr/Matis.Hudon/Shape.html"
#url_slides = "#"
url_video = "https://youtu.be/ZuEvoZXgOik?list=UUb_VXTBD3haz-P7P0f_Bi8A"

#[[url_custom]]
#name = "Custom Link"
#url = "http://www.example.org"

+++
