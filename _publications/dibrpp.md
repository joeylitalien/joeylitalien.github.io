---
layout: pub

short-title: DIB-R++
title: "DIB-R++: Learning to Predict Lighting and Material with a Hybrid Differentiable Renderer"
format-title: "DIB-R++: Learning to Predict Lighting and Material with a Hybrid Differentiable Renderer"
summary:
authors:
    - author:
        name: Wenzheng Chen
        institution: "NVIDIA, University of Toronto & Vector Institute"
        link: http://www.cs.toronto.edu/~wenzheng/
    - author:
        name: Joey Litalien
        institution: McGill University†
        link: https://joeylitalien.github.io
    - author:
        name: Jun Gao
        institution: "NVIDIA, University of Toronto & Vector Institute"
        link: http://www.cs.toronto.edu/~jungao/
    - author:
        name: Zian Wang
        institution: "NVIDIA, University of Toronto & Vector Institute"
        link: https://scholar.google.de/citations?user=rFd-DiAAAAAJ
    - author:
        name: Clément Fuji Tsang
        institution: NVIDIA
        link: https://scholar.google.ca/citations?user=U3fx-w4AAAAJ&hl=en
    - author:
        name: Sameh Khamis
        institution: NVIDIA
        link: https://www.samehkhamis.com/
    - author:
        name: Or Litany
        institution: NVIDIA
        link: https://orlitany.github.io/
    - author:
        name: Sanja Fidler
        institution: "NVIDIA, University of Toronto & Vector Institute"
        link: https://www.cs.toronto.edu/~fidler/

internship-note: Work done during an internship at NVIDIA
journal: Neural Information Processing Systems
journal-note: NeurIPS
spotlight-note:
volume: X
number: X
article-no: XX
doi:
month: December
year: 2021

thumbnail: /assets/thumbnails/dibrpp-thumb.png
thumbnail-video: #
teaser: /assets/teasers/dibrpp-teaser.png
teaser-caption: "Prediction on LSUN Dataset (Cars): DIB-R++, trained on StyleGAN dataset, can generalize well to real images. Moreover, it also predicts correct high specular lighting directions and usable, clean textures."

abstract: |
    We consider the challenging problem of predicting intrinsic object properties from a single image by exploiting differentiable renderers. Many previous learning-based approaches for inverse graphics adopt rasterization-based renderers and assume naive lighting and material models, which often fail to account for non-Lambertian, specular reflections commonly observed in the wild. In this work, we propose DIB-R++, a hybrid differentiable renderer which supports these photorealistic effects by combining rasterization and ray-tracing, taking the advantage of their respective strengths—speed and realism. Our renderer incorporates environmental lighting and spatially-varying material models to efficiently approximate light transport, either through direct estimation or via spherical basis functions. Compared to more advanced physics-based differentiable renderers leveraging path tracing, DIB-R++ is highly performant due to its compact and expressive shading model, which enables easy integration with learning frameworks for geometry, reflectance and lighting prediction from a single image without requiring any ground-truth. We experimentally demonstrate that our approach achieves superior material and lighting disentanglement on synthetic and real data compared to existing rasterization-based approaches and showcase several artistic applications including material editing and relighting.

# video:

acknowledgements: #

downloads:
    published: True
    paper:
        file: /assets/dibrpp/dibrpp.pdf
        size: 2.9MB
        file-lowres: #
        size-lowres: #
    arxiv:
        url: https://arxiv.org/abs/2111.00140
    main:
        url: https://nv-tlabs.github.io/DIBRPlus
    doi:
        url: https://papers.nips.cc/paper/2021/hash/c0f971d8cd24364f2029fcb9ac7b71f5-Abstract.html
    supplementary:
        file: #
        size: #
        url: #
    slides:
        file: #
        size: #
        file-key: #
        size-key:
    video:
        file: #
        size: #
        url: #
    talk-video:
        url: #
        venue: #
    code:
        published: false
        file: #
        size: #
        url: #
    bibtex:
        file: /assets/dibrpp/dibrpp.bib
        size: 0.5KB

tex: |
    @inproceedings{Chen:2021:DIBRPP,
        title = {{DIB-R++}: Learning to Predict Lighting and Material with a Hybrid Differentiable Renderer,
        author = {Wenzheng Chen and
                  Joey Litalien and
                  Jun Gao and
                  Zian Wang and
                  Clement Fuji Tsang and
                  Sameh Khalis and
                  Or Litany and
                  Sanja Fidler},
        year = {2021},
        journal = {Conference on Neural Information Processing Systems (NeurIPS)}
    }

tag: research
permalink: /publications/dibrpp
featured: 2
publication-date: 2112
---
