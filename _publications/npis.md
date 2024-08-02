---
layout: pub

short-title: NPIS
title: "Neural Product Importance Sampling via Warp Composition"
format-title: "Neural Product Importance Sampling via Warp Composition"
summary:
authors:
    - author:
        name: Joey Litalien
        institution: McGill University†
        link: https://joeylitalien.github.io
    - author:
        name: Miloš Hašan
        institution: Adobe Research
        link: http://www.miloshasan.net/
    - author:
        name: Fujun Luan
        institution: Adobe Research
        link: https://luanfujun.com/
    - author:
        name: Krishna Mullia
        institution: Adobe Research
        link: https://krishnamullia.com/
    - author:
        name: Iliyan Georgiev
        institution: Adobe Research
        link: https://iliyan.com/publications

internship-note: Work partly done during an internship at Adobe
journal: ACM SIGGRAPH Conference Papers
journal-note: Conditionally accepted
spotlight-note:
volume: X
number: X
article-no: XX
doi:
month: July
year: 2024

thumbnail: /assets/thumbnails/npis-thumb.png
thumbnail-video: #
teaser: /assets/teasers/npis-teaser.png
teaser-caption: |
    Our method composes a neural spline flow head warp with an emitter tail warp to achieve approximate product importance sampling of environment lighting with other terms (cosine and BRDF). Left: we apply this to cosine-weighted environment sampling on the Temple scene, demonstrating significant variance reduction over multiple importance sampling at equal rendering time. Right: we visualize the conditional distribution learned by our model at the shading point marked in green. Our learned pdf closely matches the true product. Our head warp does not have to learn the intricate details of the environment map already captured by the tail warp, and can be represented as a compact normalizing flow that can be baked for fast inference.

abstract: |
    Achieving high efficiency in modern photorealistic rendering methods hinges on using Monte Carlo sampling distributions that closely approximate the illumination integral estimated for every pixel. Samples are typically generated from a set of simple distributions, each targeting a different factor in the integrand, which are combined via multiple importance sampling. The resulting mixture distribution can be far from the actual product of all factors, leading to sub-optimal variance even for direct-illumination estimation. We present a learning-based method to efficiently importance sample illumination product integrals (e.g., the product of environment lighting and material terms) using normalizing flows. Our neural product sampler composes a flow head warp with an emitter tail warp. The small conditional head is represented by a neural spline flow, while the large unconditional tail is discretized per environment map and its evaluation is instant. If the conditioning is low-dimensional, the head warp can be discretized for even better performance. We demonstrate variance reduction over prior methods on a range of applications comprising complex geometry, materials and illumination.

# video:

acknowledgements: #

downloads:
    published: False
    paper:
        file: /assets/dibrpp/dibrpp.pdf
        size: 2.9MB
        file-lowres: #
        size-lowres: #
    arxiv:
        url: #
    main:
        url: #
    doi:
        url: #
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
        file: #
        size: #

tex: |
    @inproceedings{chen2021dibrpp,
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
permalink: /publications/npis
featured: 1
publication-date: 2407
---
