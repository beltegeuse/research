+++
title = "Shape and Reflectance from RGB-D Images using Time Sequential Illumination"
date = 2016-02-01

[extra]
authors = [
    { name = "Matis Hudon", institution = "Technicolor, IRISA, University of Rennes 1, France" }, 
    { name = "Adrien Gruson", institution = "IRISA, University of Rennes 1, France" },
    { name = "Paul Kerbiriou", institution = "Technicolor, France" },
    { name = "Remi Cozot", institution = "IRISA, University of Rennes 1, France" },
    { name = "Kadi Bouatouch", institution = "IRISA, University of Rennes 1, France" }
]

image = "RGBD.png"
image_preview = "RGBD_prev.png"
publication = "*VISAPP*, 2016."
short_description = "Method for recovering the shape with Kinect and partially controlled illumination."

download = [
    { type = "paper", url = "https://profs.etsmtl.ca/agruson/DATA/2016_RGBD-Sequential_Hudon.pdf"},
    { type = "doi", url = "http://doi.org/10.5220/0005726305320541" },
    { type = "project", url = "http://people.irisa.fr/Matis.Hudon/Shape.html" }
]

abstract = """In this paper we propose a method for recovering the shape (geometry) and the diffuse reflectance from an image (or video) using a hybrid setup consisting of a depth sensor (Kinect), a consumer camera and a partially controlled illumination (using a flash). The objective is to show how combining RGB-D acquisition with a sequential illumination is useful for shape and reflectance recovery. A pair of two images are captured: one non flashed (image under ambient illumination) and a flashed one. A pure flash image is computed by subtracting the non flashed image from the flashed image. We propose an novel and near real-time algorithm, based on a local illumination model of our flash and the pure flash image, to enhance geometry (from the noisy depth map) and recover reflectance information."""

bibtex = """@inproceedings{Hudon:2016:Shape,
  title={Shape and Reflectance from RGB-D Images using Time Sequential Illumination.},
  author={Hudon, Matis and Gruson, Adrien and Kerbiriou, Paul and Cozot, Remi and Bouatouch, Kadi},
  booktitle={VISIGRAPP (3: VISAPP)},
  year={2016},
  doi={10.5220/0005726305320541}
}"""

+++

