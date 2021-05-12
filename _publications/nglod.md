---
layout: pub

short-title: NGLOD
title: "Neural Geometric Level of Detail: Real-time Rendering with Implicit 3D Shapes"
format-title: "Neural Geometric Level of Detail:<br>Real-time Rendering with Implicit 3D Shapes"
summary: Neural SDFs, but real-time
authors:
    - author: 
        name: Towaki Takikawa
        institution: NVIDIA & University of Toronto
        link: https://tovacinni.github.io/
        order: 1
    - author: 
        name: Joey Litalien
        institution: NVIDIA & McGill University
        link: https://joeylitalien.github.io
        order: 1
    - author: 
        name: Kangxue Yin
        institution: NVIDIA
        link: https://kangxue.org/
    - author: 
        name: Karsten Kreis
        institution: NVIDIA
        link: https://scholar.google.de/citations?user=rFd-DiAAAAAJ
    - author:
        name: Charles Loop
        institution: NVIDIA
        link: https://research.nvidia.com/person/charles-loop/
    - author: 
        name: Derek Nowrouzezahrai
        institution: McGill University
        link: http://www.cim.mcgill.ca/~derek/
    - author: 
        name: Alec Jacobson
        institution: University of Toronto
        link: https://www.cs.toronto.edu/~jacobson/
    - author: 
        name: Morgan McGuire
        institution: NVIDIA & McGill University
        link: https://casual-effects.com/
    - author: 
        name: Sanja Fidler
        institution: NVIDIA, University of Toronto & Vector Institute
        link: https://www.cs.toronto.edu/~fidler/

journal: Computer Vision and Pattern Recognition
journal-note: CVPR
volume: 1
number: 1
article-no: 1
doi: 
month: January
year: 2021

thumbnail: /assets/thumbnails/nglod-thumb.png
thumbnail-video: /assets/thumbnails/nglod-thumb.mp4
teaser: /assets/teasers/nglod-teaser.png
teaser-caption: "We are able to fit shapes of varying complexity, style, scale, with consistently good quality, while being able to leverage the geometry for shading, ambient occlusion, and even shadows with secondary rays."

abstract: |
    Neural signed distance functions (SDFs) are emerging as an effective representation for 3D shapes. SDFs encode 3D surfaces with a function of position that returns the closest distance to a surface. State-of-the-art methods typically encode the SDF with a large, fixed-size neural network to approximate complex shapes with implicit surfaces. Rendering these large networks is, however, computationally expensive since it requires many forward passes through the network for every pixel, making these representations impractical for real-time graphics applications. We introduce an efficient neural representation that, for the first time, enables real-time rendering of high-fidelity neural SDFs, while achieving state-of-the-art geometry reconstruction quality. We represent implicit surfaces using an octree-based feature volume which adaptively fits shapes with multiple discrete levels of detail (LODs), and enables continuous LOD with SDF interpolation. We further develop an efficient algorithm to directly render our novel neural SDF representation in real-time by querying only the necessary LODs with sparse octree traversal. We show that our representation is 2-3 orders of magnitude more efficient in terms of rendering speed compared to previous works. Furthermore, it produces state-of-the-art reconstruction quality for complex shapes under both 3D geometric and 2D image-space metrics.

# video: 

acknowledgements: We would like to thank 
    <a href="https://scholar.google.com/citations?user=PDvW5o4AAAAJ&hl=en">Jean-Francois Lafleche</a>, 
    <a href="https://www.petershirley.com/">Peter Shirley</a>, 
    <a href="https://kevincxie.github.io/">Kevin Xie</a>, 
    <a href="http://granskog.xyz/">Jonathan Granskog</a>, 
    <a href="https://research.nvidia.com/person/alex-evans">Alex Evans</a>, and 
    <a href="https://www.linkedin.com/in/alexbie98">Alex Bie</a> at NVIDIA for interesting discussions throughout the project. 
    We also thank 
    <a href="https://www.petershirley.com/">Peter Shirley</a>, 
    <a href="https://research.nvidia.com/person/zander-majercik">Alexander Majercik</a>, 
    <a href="https://research.nvidia.com/person/jacob-munkberg">Jacob Munkberg</a>, 
    <a href="https://luebke.us/">David Luebke</a>,
    <a href="https://scholar.google.com/citations?user=VVIAoY0AAAAJ&hl=en">Jonah Philion</a> and 
    <a href="http://www.cs.toronto.edu/~jungao/">Jun Gao</a> for their help with paper editing.

downloads:
    published: True
    paper:
        file: /assets/nglod/nglod.pdf
        size: 6.2MB
        file-lowres: #
        size-lowres: #
    arxiv:
        url: https://arxiv.org/abs/2101.10994
    main:
        url: https://nv-tlabs.github.io/nglod/
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
        url: https://www.youtube.com/watch?v=Pi7W6XrFtMs
        venue: Toronto Geometry Colloquium
    code:
        published: True
        file: #
        size: #
        url: https://github.com/nv-tlabs/nglod
    bibtex:
        file: /assets/nglod/nglod.bib
        size: 0.5KB

tex: |
    @article{takikawa2021nglod,
        title = {Neural Geometric Level of Detail: Real-time Rendering with Implicit {3D} Shapes}, 
        author = {Towaki Takikawa and
                  Joey Litalien and 
                  Kangxue Yin and 
                  Karsten Kreis and 
                  Charles Loop and 
                  Derek Nowrouzezahrai and 
                  Alec Jacobson and 
                  Morgan McGuire and 
                  Sanja Fidler},
        year = {2021},
        journal = {arXiv preprint arXiv:2101.10994}
    }

tag: research
permalink: /publications/nglod
featured: 1
---
