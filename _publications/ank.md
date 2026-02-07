---
layout: pub

short-title: ANK
title: "Adaptive Neural Kernels for Gradient-domain Rendering"
format-title: "Adaptive Neural Kernels for Gradient-domain Rendering"
summary:
authors:
    - author:
        name: Matthieu Josse
        institution: École polytechnique
        link: https://www.linkedin.com/in/matthieu-josse-948728228/
    - author:
        name: Joey Litalien
        institution: Independent†
        link: https://joeylitalien.com
    - author:
        name: Adrien Gruson
        institution: École de technologie supérieure (ÉTS)
        link: https://profs.etsmtl.ca/agruson

internship-note: Work partly done during time at McGill University, Canada.
journal: ACM SIGGRAPH Asia 2025
journal-note: Conference Proceedings
spotlight-note:
volume: 1
number: 1
article-no: 1
doi: 10.1145/3680528.3687566
month: December
year: 2025

thumbnail: /assets/thumbnails/ank-thumb.png
thumbnail-video: #
teaser: /assets/teasers/ank-teaser.png
teaser-caption: |
    Equal-time comparison between our adaptive kernel, the structure-adaptive kernel <a href="https://dl.acm.org/doi/10.1145/2661229.2661291">[Manzi et al. 2014]</a>, and the standard cross-shaped kernel. All methods use gradients produced by gradient-domain path tracing with path reconnection.

abstract: |
    Monte Carlo methods are a cornerstone of physics-based light transport simulations, valued for their ability to produce high-quality photorealistic images. These stochastic methods often suffer from variance, resulting in undesirable noise in the rendered images. Gradient-domain rendering (GDR) techniques mitigate this problem by estimating unbiased image-space gradients via so-called shift-mapping operators. While these mappings are computationally efficient, they can yield high-variance gradients—and thus poor reconstruction quality—when applied to pixels with wildly different integrals. We tackle this challenge by dynamically selecting the optimal set of neighboring pixels for applying shift-mapping under random sequence replay. Key to our approach is a differentiable sorting network that softly ranks the output of a convolutional neural network conditioned on input sample features for weighted reconstruction. This module is carefully rigidified over time to converge to a hard top-<i>k</i> selection, allowing end-to-end optimization with respect to the reconstruction error. Our method is versatile and can be jointly optimized with other adaptive sampling strategies. We demonstrate variance reduction over other traditional adaptive gradient-domain methods across scenes of varying radiometric complexity.

# video:

acknowledgements: #

downloads:
    published: True
    paper:
        file: /assets/ank/ank_gdr.pdf
        size: 11.9MB
        file-lowres: #
        size-lowres: #
    arxiv:
        url:
    main:
        url: 
    doi:
        url: https://doi.org/10.1145/3757377.3763920
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
        url: #
        size: #
    code:
        published: true
        file: #
        size: #
        url: https://github.com/MattJosse/adaptive-neural-kernel
    bibtex:
        file: /assets/ank/ank.bib
        size: 0.3KB

tex: |
    @inproceedings{Josse:2025:ANK,
        title = {Adaptive Neural Kernels for Gradient-domain Rendering},
        author = {Matthieu Josse and
                  Joey Litalien and
                  Adrien Gruson},
        journal = {ACM SIGGRAPH Asia 2025 Conference Proceedings},
        year = {2025},
        month = dec,
        doi = {10.1145/3680528.3687566}
    }

tag: research
permalink: /publications/ank
featured: 2
publication-date: 2512
---