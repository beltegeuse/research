+++
date = 2013-10-01
title = "Eye-Centred Color Adaptation in Global Illumination"

[extra]
abstract_short = "In this paper, we propose a new color adaptation method well suited to global illumination. This method estimates the adaptation color by averaging the irradiance color arriving at the eye. Unlike other existing methods, our approach is not limited to the view frustrum."
authors = ["A Gruson", "M Ribardiere", "R Cozot"]
image = "eyecenter.png"
image_preview = "eyecenter_prev.png"
math = true
publication_types = ["2"]
publication = "*Pacific Graphics*, 2013."
selected = true

url = [["PDF","http://onlinelibrary.wiley.com/doi/10.1111/cgf.12218/abstract"]]

+++

### Abstract

Color adaptation is a well known ability of the human visual system (HVS). Colors are perceived as constant even though the illuminant color changes. Indeed, the perceived color of a diffuse white sheet of paper is still white even though it is illuminated by a single orange tungsten light, whereas it is orange from a physical point of view. Unfortunately global illumination algorithms only focus on the physics aspects of light transport. The ouput of a global illuminantion engine is an image which has to undergo chromatic adaptation to recover the color as perceived by the HVS. In this paper, we propose a new color adaptation method well suited to global illumination. This method estimates the adaptation color by averaging the irradiance color arriving at the eye. Unlike other existing methods, our approach is not limited to the view frustrum, as it considers the illumination from all the scene. Experiments have shown that our method outperforms the state of the art methods.

### Video
<video width="320" height="240" controls>
  <source src="http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2013_whitebalancing/video.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>