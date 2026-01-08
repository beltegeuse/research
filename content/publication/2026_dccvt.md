+++
title = "DCCVT: Differentiable Clipped Centroidal Voronoi Tessellation"
date = 2026-01-08

[extra]
authors = [
    { name = "Wylliam Cantin Charawi", institution = "École de Technologie Supérieure"},
    { name = "Adrien Gruson", institution = "École de Technologie Supérieure" },
    { name = "Jane Wu", institution = "Standford" },
    { name = "Christian Desrosiers", institution = "École de Technologie Supérieure" },
    { name = "Diego Thomas", institution = "Kyushu University" }
]
join_first = false

publication = "*3DV*, 2026."
image = "DCCVT_banner.png"
image_preview = "DCCVT_prev.png"
short_description = "Differentiable Voronoi mesh reconstruction from point clouds"

download = [
    { type = "project", url = "https://wylliamcantincharawi.dev/DCCVT.github.io/" }
]

abstract = """While Marching Cubes (MC) and Marching Tetrahedra (MTet) are widely adopted in 3D reconstruction pipelines due to their simplicity and efficiency, their differentiable variants remain suboptimal for mesh extraction. This often limits the quality of 3D meshes reconstructed from point clouds or images in learning-based frameworks. In contrast, clipped CVTs offer stronger theoretical guarantees and yield higher-quality meshes. However, the lack of a differentiable formulation has prevented their integration into modern machine learning pipelines. To bridge this gap, we propose DCCVT, a differentiable algorithm that extracts high-quality 3D meshes from noisy signed distance fields (SDFs) using clipped CVTs. We derive a fully differentiable formulation for computing clipped CVTs and demonstrate its integration with deep learning-based SDF estimation to reconstruct accurate 3D meshes from input point clouds. Our experiments with synthetic data demonstrate the superior ability of DCCVT against state-of-the-art methods in mesh quality and reconstruction fidelity."""

bibtex = """@inproceedings{charawi20263dv,
  author    = {Charawi, Wylliam Cantin and Gruson, Adrien and Wu, Jane and Desrosiers, Christian and Thomas, Diego},
  title     = {DCCVT: Differentiable Clipped Centroidal Voronoi
              Tessellation},
  booktitle = {Proceedings of the 15th International Conference on 3D Vision (3DV)},
  year      = {2026},
  month     = {March},
  address   = {Vancouver, BC, Canada}
}
"""

+++