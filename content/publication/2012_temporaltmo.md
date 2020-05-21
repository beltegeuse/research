+++
date = 2012-10-01
title = "Temporal Coherency for Video Tone Mapping"

[extra]
authors = [
    { name = "Ronan Boitard", institution = "Technicolor, IRISA, University of Rennes 1, France" },
    { name = "Kadi Bouatouch", institution = "IRISA, University of Rennes 1, France" },
    { name = "Remi Cozot", institution = "IRISA, University of Rennes 1, France" },
    { name = "Dominique Thoreau", institution = "Technicolor, France" },
    { name = "Adrien Gruson", institution = "IRISA, University of Rennes 1, France" }
]

image = "temporal_video.png"
image_preview = "temporal_video_prev.png"
publication = "*SPIE*, 2012."
short_description = "Tone mapping achieving more stable result with video."

download = [
    { type = "paper", url = "http://www.ece.ubc.ca/~rboitard/articles/2012/Boitard%20et%20al.-2012-Temporal%20Coherency%20for%20Video%20Tone%20Mapping.pdf"},
    { type = "doi", url = "https://doi.org/10.1117/12.929600" }
]

+++

### Abstract

Tone Mapping Operators (TMOs) aim at converting real world high dynamic range (HDR) images captured with HDR cameras, into low dynamic range (LDR) images that can be displayed on LDR displays.  Several TMOs have been proposed over the last decade, from the simple global mapping to the more complex one simulating the human vision system.  While these solutions work generally well for still pictures, they are usually less effcient for video sequences as they are source of visual artifacts.  Only few of them can be adapted to cope with a sequence of images.  In this paper we present a major problem that a static TMO usually encounters while dealing with video sequences, namely the temporal coherency.  Indeed, as each tone mapper deals with each frame separately, no  temporal  coherency  is  taken  into  account  and  hence  the  results  can  be  quite  disturbing  for  high  varying dynamics in a video.  We propose a temporal coherency algorithm that is designed to analyze a video as a whole, and  from  its  characteristics  adapts  each  tone  mapped  frame  of  a  sequence  in  order  to  preserve  the  temporal coherency.  This temporal coherency algorithm has been tested on a set of real as well as Computer Graphics Image (CGI) content and put in competition with several algorithms that are designed to be time-dependent. Results show that temporal coherency preserves the overall contrast in a sequence of images.  Furthermore, this technique is applicable to any TMO as it is a post-processing that only depends on the used TMO.