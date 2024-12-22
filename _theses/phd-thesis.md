---
layout: pub

short-title: PhD
title: Statistical and Learning‑based Methods for High‑performance Rendering
format-title: Statistical and Learning‑based Methods for High‑performance Rendering
authors:
    - author:
        name: Joey Litalien
        institution: McGill University
        link: https://joeylitalien.github.io
jury:
    - author:
        name: Wojciech Jarosz
        link: https://cs.dartmouth.edu/~wjarosz/
    - author:
        name: Di Wu 
        link: https://scholar.google.ca/citations?user=IbcoTsgAAAAJ&hl=en
    - author:
        name: Paul G. Kry
        link: https://www.cs.mcgill.ca/~kry/
    - author:
        name: James J. Clark
        link: https://www.cim.mcgill.ca/~clark/

journal: Doctoral thesis
journal-note: Ph.D.
spotlight-note:
volume:
number:
month: December
year: 2024

thumbnail: /assets/thumbnails/phdthesis-thumb.png
teaser: /assets/teasers/phdthesis-teaser.png
teaser-caption: >
    <i>Left:</i> Rendering photorealistic scenes requires a computationally intensive light transport simulation, which can make interactive previewing difficult as artists must wait for the variance (noise) to vanish. Reducing the variance of Monte Carlo rendering estimators remove some of this burden. <i>Right:</i> Using signed distance fields as a scene representation can facilitate the creation of immersive environments. Living room scene designed by IC-Design; island scene sculpted by Joshua Eiten in Adobe Substance 3D Modeler.

abstract: >
    Capturing and synthesizing the appearance of real world phenomena is a long-standing goal of computer graphics. The gamut of rendering applications is remarkably large, ranging from real-time visualization of immersive environments in virtual reality to physics-based light transport simulations for animated feature films. Despite tremendous progress in improving the workflow of digital artists, the main bottleneck to their productivity remains content creation, as a vast amount of manual labor is still required to author photorealistic 3D scenes with detailed geometry, emission profiles and materials. This thesis investigates statistical and machine learning-based methods to circumvent (parts of) this tedious creation process. We present three practical rendering techniques, each targeting complementary aspects of the rendering cycle.<br>
    <br>
    First, we extend the framework of delayed rejection Markov chain Monte Carlo to primary sample space Metropolis light transport (MLT) and introduce a two-stage proposal mechanism that automatically balances local exploration and computational efficiency. Our method, called delayed rejection Metropolis light transport (DRMLT), exploits prioritization by proposing bolder or less costly transitions first before falling back on more timid or expensive kernels upon failure. We show how our sampler is general and robust by deploying it on radiometrically complex scenes, showcasing improved convergence over prior MLT-based techniques.<br>
    <br>
    Second, we propose a learning-based Monte Carlo method to efficiently importance sample illumination products (e.g., the product of environment lighting and material) using normalizing flows. Our neural product sampler composes a flow head warp with an emitter tail warp: the small conditional head is represented by a neural spline flow, while the large unconditional tail is discretized per environment map and its evaluation is instant. We show that imbuing our model with an near-exact emitter warp is an effective inductive bias for neural product sampling and demonstrate significant variance reduction over previous methods on a range of rendering applications.<br>
    <br>
    Finally, we present neural geometric level of detail (NGLoD), an efficient neural representation that, for the first time, enables real-time rendering of high-fidelity neural signed distance fields (SDFs) while achieving high reconstruction quality. Here, we represent implicit surfaces using an octree-based feature volume which adaptively fits shapes with multiple discrete levels of detail (LoDs) and enables continuous LoD with SDF interpolation. We further develop an efficient GPU-based algorithm to interactively render our neural SDF representation via sparse octree ray traversal. We show how NGLoD can represent 3D shapes in a compressed format with higher visual fidelity than traditional methods.


downloads:
    published: False
    paper:
        file: /assets/phd-thesis/thesis.pdf
        size: X.XMB
        file-lowres: /assets/phd-thesis/thesis-lowres.pdf
        size-lowres: X.XMB
    bibtex:
        file:
        size:

tex: |
    @phdthesis{Litalien:2024:Thesis,
       author = {Litalien, Joey},
       title = {Statistical and Learning‑based Methods for High‑performance Rendering},
       school = {McGill University}
       year = {2024},
       month = dec
    }

tag: research
permalink: /publications/phdthesis
featured: 1
publication-date: 2501
---
