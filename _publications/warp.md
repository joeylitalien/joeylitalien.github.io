---
layout: pub

short-title: WARP
title: "Neural Product Importance Sampling via Warp Composition"
format-title: "Neural Product Importance Sampling <br>via Warp Composition"
summary:
authors:
    - author:
        name: Joey Litalien
        institution: McGill University†
        link: https://joeylitalien.github.io
    - author:
        name: Miloš Hašan
        institution: Adobe Research
        link: http://www.miloshasan.net
    - author:
        name: Fujun Luan
        institution: Adobe Research
        link: https://luanfujun.com
    - author:
        name: Krishna Mullia
        institution: Adobe Research
        link: https://krishnamullia.com
    - author:
        name: Iliyan Georgiev
        institution: Adobe Research
        link: https://iliyan.com

internship-note: Work partly done during an internship at Adobe Research, UK
journal: ACM SIGGRAPH Asia 2024
journal-note: Conference Proceedings
spotlight-note:
volume: 1
number: 1
article-no: 1
doi: 10.1145/3680528.3687566
month: December
year: 2024

thumbnail: /assets/thumbnails/warp-thumb.png
thumbnail-video: #
teaser: /assets/teasers/warp-teaser-transparent.png
teaser-caption: |
    Our method composes a neural spline flow <i>head warp</i> with an emitter <i>tail warp</i> to achieve approximate product importance sampling of environment lighting with other terms (cosine and BRDF). Applied to cosine-weighted environment sampling on the Temple scene, we demonstrate significant variance reduction over multiple importance sampling (MIS) at equal rendering time (35 ms, 4 spp). We also visualize the conditional distribution learned by our model at the shading point marked in green. Our learned PDF closely matches the true (unshadowed) product. Our head warp does not have to learn the intricate details of the environment map already captured by the tail warp, and can be represented as a compact normalizing flow that can be baked for fast inference.

abstract: |
    Achieving high efficiency in modern photorealistic rendering hinges on using Monte Carlo sampling distributions that closely approximate the illumination integral estimated for every pixel. Samples are typically generated from a set of simple distributions, each targeting a different factor in the integrand, which are combined via multiple importance sampling. The resulting mixture distribution can be far from the actual product of all factors, leading to sub-optimal variance even for direct-illumination estimation. We present a learning-based method that uses normalizing flows to efficiently importance sample illumination product integrals, e.g., the product of environment lighting and material terms. Our sampler composes a flow head warp with an emitter tail warp. The small conditional head warp is represented by a neural spline flow, while the large unconditional tail is discretized per environment map and its evaluation is instant. If the conditioning is low-dimensional, the head warp can be also discretized to achieve even better performance. We demonstrate variance reduction over prior methods on a range of applications comprising complex geometry, materials and illumination.

# video:

acknowledgements: #

downloads:
    published: True
    paper:
        file: /assets/warp/neural_warp.pdf
        size: 13.2MB
        file-lowres: #
        size-lowres: #
    arxiv:
        url: https://arxiv.org/abs/2409.18974
    main:
        url: 
    doi:
        url: https://doi.org/10.1145/3680528.3687566
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
    ff-video:
        url: /assets/warp/neural_warp_fast_forward.mp4
        size: 2.6MB
    code:
        published: false
        file: #
        size: #
        url: hhttps://github.com/joeylitalien/neural-warp
    bibtex:
        file: /assets/warp/warp.bib
        size: 0.4KB

tex: |
    @inproceedings{Litalien:2024:Warp,
        title = {Neural Product Importance Sampling via Warp Composition},
        author = {Joey Litalien and
                  Miloš Hašan and
                  Fujun Luan and
                  Krishna Mullia and
                  Iliyan Georgiev},
        journal = {ACM SIGGRAPH Asia 2024 Conference Proceedings},
        year = {2024},
        month = dec,
        doi = {10.1145/3680528.3687566}
    }

tag: research
permalink: /publications/warp
featured: 2
publication-date: 2412
---
