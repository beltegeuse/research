+++
title = "Shape and Reflectance from RGB-D Images using Time Sequential Illumination"
date = 2016-02-01

[extra]
authors = ["M Hudon", "A Gruson", "P Kerbiriou", "R Cozot", "K Bouatouch"]

image = "RGBD.png"
image_preview = "RGBD_prev.png"
math = true
publication_types = ["2"]
publication = "*VISAPP*, 2016."
selected = false

url = [["PDF", "http://beltegeuse.s3-website-ap-northeast-1.amazonaws.com/research/2016_RGBD-Sequential_Hudon.pdf"],
    ["Project page", "http://people.irisa.fr/Matis.Hudon/Shape.html"]]

+++

### Abstract

In this paper we propose a method for recovering the shape (geometry) and the diffuse reflectance from an image (or video) using a hybrid setup consisting of a depth sensor (Kinect), a consumer camera and a partially controlled illumination (using a flash). The objective is to show how combining RGB-D acquisition with a sequential illumination is useful for shape and reflectance recovery. A pair of two images are captured: one non flashed (image under ambient illumination) and a flashed one. A pure flash image is computed by subtracting the non flashed image from the flashed image. We propose an novel and near real-time algorithm, based on a local illumination model of our flash and the pure flash image, to enhance geometry (from the noisy depth map) and recover reflectance information.
