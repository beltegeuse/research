+++
abstract = "Tone Mapping Operators (TMOs) aim at converting real world high dynamic range (HDR) images captured with HDR cameras, into low dynamic range (LDR) images that can be displayed on LDR displays.  Several TMOs have been proposed over the last decade, from the simple global mapping to the more complex one simulating the human vision system.  While these solutions work generally well for still pictures, they are usually less effcient for video sequences as they are source of visual artifacts.  Only few of them can be adapted to cope with a sequence of images.  In this paper we present a major problem that a static TMO usually encounters while dealing with video sequences, namely the temporal coherency.  Indeed, as each tone mapper deals with each frame separately, no  temporal  coherency  is  taken  into  account  and  hence  the  results  can  be  quite  disturbing  for  high  varying dynamics in a video.  We propose a temporal coherency algorithm that is designed to analyze a video as a whole, and  from  its  characteristics  adapts  each  tone  mapped  frame  of  a  sequence  in  order  to  preserve  the  temporal coherency.  This temporal coherency algorithm has been tested on a set of real as well as Computer Graphics Image (CGI) content and put in competition with several algorithms that are designed to be time-dependent. Results show that temporal coherency preserves the overall contrast in a sequence of images.  Furthermore, this technique is applicable to any TMO as it is a post-processing that only depends on the used TMO."
authors = ["R Boitard", "K Bouatouch", "R Cozot", "D Thoreau", "A Gruson"]
date = "2012-10-01"
image = "publications/temporal_video.png"
image_preview = ""
math = true
publication = "In *SPIE*, 2012."
publication_short = "In *SPIE 2012*"
selected = false
title = "Temporal Coherency for Video Tone Mapping"
#url_code = "#"
#url_dataset = "#"
url_pdf = "http://www.ece.ubc.ca/~rboitard/articles/2012/Boitard%20et%20al.-2012-Temporal%20Coherency%20for%20Video%20Tone%20Mapping.pdf"
#url_project = "http://people.irisa.fr/Matis.Hudon/Shape.html"
#url_slides = "#"
#url_video = "#"

#[[url_custom]]
#name = "Custom Link"
#url = "http://www.example.org"

+++
