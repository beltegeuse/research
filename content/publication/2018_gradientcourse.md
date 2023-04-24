+++
date = 2018-11-01
title = "Light Transport Simulation in the Gradient Domain"

[extra]
authors = [
    { name = "Binh-Son Hua", institution = "The University of Tokyo, Japan" },
    { name = "Adrien Gruson", institution = "The University of Tokyo, JFLI, Japan" },
    { name = "Matthias Zwicker", institution = "University of Maryland, USA" },
    { name = "Toshiya Hachisuka", institution = "The University of Tokyo, Japan" }
]

image = "GradientCourse.png"
image_preview = "GradientCourse_prev.png"
publication = "*SIGGRAPH Asia (Course)*, 2018."
short_description = "Course on gradient-domain rendering."

download = [
    { type = "project", url = "https://data.adrien-gruson.com/research/2018_GradientCourse/" },
    { type = "doi", url = "https://doi.org/10.1145/3277644.3277761"},
    { type = "additional", desc = "Web interactive comparision", url = "https://data.adrien-gruson.com/research/2018_GVPM/comparison/index.html"}
]

abstract = """Despite the wide adoption in film production and animation industry nowadays, Monte Carlo light transport simulation is still prone to producing noisy images within short rendering time. Accelerating the convergence of Monte Carlo rendering without sacrificing its accuracy is by far a challenging task. In this course, we will learn about gradient-domain light transport simulation, a recent family of techniques in physically based rendering introduced in the past five years that can accelerate traditional Monte Carlo rendering up to approximately an order of magnitude based on gradient estimation and image reconstruction. Particularly, we will introduce the fundamentals of gradient-domain rendering with gradient-domain path tracing, and then extend the discussion to gradient-domain bidirectional path tracing and photon density estimation. We also discuss volume rendering in the gradient domain before diving into advanced topics in recent state-of-the-art papers in this direction. We further discuss tips and tricks in open-source implementations of such algorithms, and provide ideas for future research directions."""

bibtex = """@incollection{Hua:2018:GradientCourse,
  title={Light transport simulation in the gradient domain},
  author={Hua, Binh-Son and Gruson, Adrien and Zwicker, Matthias and Hachisuka, Toshiya},
  booktitle={SIGGRAPH Asia 2018 Courses},
  year={2018},
  doi={10.1145/3277644.3277761}
}"""

+++
