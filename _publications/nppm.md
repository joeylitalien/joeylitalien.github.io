---
layout: pub

short-title: NPPM
title: "Neural Progressive Photon Mapping"
format-title: "Neural Progressive Photon Mapping"
summary:
authors:
    - author:
        name: Justin Benoist
        institution: École de technologie supérieure (ÉTS)
        link: https://www.linkedin.com/in/justin-benoist/
    - author:
        name: Joey Litalien
        institution: Independent†
        link: https://joeylitalien.com
    - author:
        name: Adrien Gruson
        institution: École de technologie supérieure (ÉTS)
        link: https://profs.etsmtl.ca/agruson

internship-note: Work partly done during time at McGill University, Canada.
journal: Eurographics 2026
journal-note: Computer Graphics Forum
spotlight-note:
volume: 1
number: 1
article-no: 1
doi: #
month: February
year: 2026

thumbnail: /assets/thumbnails/nppm-thumb.png
thumbnail-video: #
teaser: /assets/teasers/nppm-teaser.png
teaser-caption: |
    Equal-time comparison (15 seconds) between our neural progressive photon mapping (NPPM), SPPM and CPPM on the <i>Crab DoF</i> scene with depth of field. The superscripts <i>α</i> and <i>β</i> respectively refer to the different radius reduction policy used by the two baseline methods, which we incorporate atop NPPM. Our technique reduces the overall bias compared to its nonneural counterparts, capturing sharper caustics on most of the scene. False color error shows the MRSE metric.

abstract: |
    Photon density estimation is a robust solution for estimating complex light transport, such as those involving caustics and pure specular interactions. The shape and bandwidth of the density kernel are both crucial in achieving optimal performance. Recently, density kernels directly predicted by neural networks from local photon statistics have shown improved reconstruction results for small numbers of photons. The direct weight prediction approach of these methods, however, is fundamentally incompatible with consistent estimators as it does not allow for direct control over bias and variance. We address this problem by relying on a simpler yet effective <i>analytical</i> kernel, also inferred by a neural network. Unlike prior work, our technique supports progressive schemes by design, hence unlocking a large variety of applications such as stochastic photon mapping. Our method is fast, trivial to train and demonstrates state-of-the-art caustics reconstruction at equal-time over other photon mapping techniques.

# video:

acknowledgements: #

downloads:
    published: True
    paper:
        file: /assets/nppm/nppm.pdf
        size: 9.2MB
        file-lowres: #
        size-lowres: #
    arxiv:
        url:
    main:
        url: 
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
    ff-video:
        url: #
        size: #
    code:
        published: false
        file: #
        size: #
        url: #
    bibtex:
        file: /assets/nppm/nppm.bib
        size: 0.3KB

tex: |
    @inproceedings{Benoist:2026:NPPM,
        title = {Neural Progressive Photon Mapping},
        author = {Justin Benoist and
                  Joey Litalien and
                  Adrien Gruson},
        journal = {Computer Graphics Forum},
        year = {2026},
        month = feb,
        doi = {XX.XXXX/XXXXXXXX.XXXX.XXXXX}
    }

tag: research
permalink: /publications/nppm
featured: 1
publication-date: 2602
---
