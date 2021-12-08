+++
title = "A Survey on Gradient-Domain Rendering"
date = 2019-03-12

[extra]
authors = [
    { name = "Binh-Son Hua", institution = "The University of Tokyo, Japan" },
    { name = "Adrien Gruson", institution = "The University of Tokyo, JFLI, Japan" },
    { name = "Victor Petitjean", institution = "Delft University of Technology, Netherlands" },
    { name = "Matthias Zwicker", institution = "University of Maryland, USA" }, 
    { name = "Derek Nowrouzezahrai", institution = "McGill University, Canada" },
    { name = "Elmar Eisemann", institution = "Delft University of Technology, Netherlands" },
    { name = "Toshiya Hachisuka", institution = "The University of Tokyo, Japan" }
]
join_first = true

image = "gradientdomain_star.jpg"
image_preview = "gradientdomain_star_prev.png"
publication = "*Eurographics (STAR)*, 2019."
short_description = "Survey on gradient-domain rendering."

download = [
    { type = "project", url = "https://adrien-gruson.com/research/2019_GradientSTAR/"},
    { type = "doi", url = "https://doi.org/10.1111/cgf.13652" },
    { type = "code", url = "https://github.com/gradientpm/gradient-mts" } 
]

abstract = """Monte Carlo methods for physically-based light transport simulation are broadly adopted in film productions and animation/visual effects industries. Monte Carlo methods, however, often result in noisy images and have slow convergence. As such, improving the convergence of Monte Carlo rendering remains an important open problem. Gradient-domain light transport is a recent family of techniques that can accelerate Monte Carlo rendering by up to an order of magnitude, leveraging a gradient-based estimation and a reformulation of the rendering problem as an image reconstruction. This state of the art report comprehensively elaborates the fundamentals of gradient-domain rendering, as well as the specifics behind gradient-domain uni- and bidirectional path tracing and gradient-domain photon density estimation. We also discuss various image reconstruction schemes which are important components of gradient-domain rendering. Finally, we benchmark various gradient-domain techniques against state-of-the-art denoising methods before discussing open problems."""

bibtex = """@inproceedings{Hua:2019:SurveyGradient,
  title={A Survey on Gradient-Domain Rendering},
  author={Hua, Binh-Son and Gruson, Adrien and Petitjean, Victor and Zwicker, Matthias and Nowrouzezahrai, Derek and Eisemann, Elmar and Hachisuka, Toshiya},
  booktitle={Computer Graphics Forum},
  volume={38},
  year={2019},
  doi={10.1111/cgf.13652}
}"""

+++
