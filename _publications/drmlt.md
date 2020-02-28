---
layout: pub

short-title: DRMLT
title: Delayed Rejection Metropolis Light Transport
authors:
    - author: 
        name: Damien Rioux-Lavoie
        institution: McGill University
        link:
        order: 1
    - author: 
        name: Joey Litalien
        institution: McGill University
        link: https://joeylitalien.github.io
        order: 1
    - author: 
        name: Adrien Gruson
        institution: McGill University
        link: https://beltegeuse.github.io/research/
    - author: 
        name: Toshiya Hachisuka
        institution: The University of Tokyo
        link: https://www.ci.i.u-tokyo.ac.jp/~hachisuka/
    - author: 
        name: Derek Nowrouzezahrai
        institution: McGill University
        link: http://www.cim.mcgill.ca/~derek/

journal: ACM Transactions on Graphics
journal-note: To be presented at SIGGRAPH
volume: X
number: XX
month: XX
year: 2020

thumbnail: /assets/thumbnails/drmlt-thumb.png
teaser: /assets/teasers/drmlt-teaser.png
teaser-caption: "We generalize the Metropolis–Hastings algorithm with delayed rejection: our <i>delayed rejection Metropolis light transport</i> (DRMLT) method selectively applies different mutation strategies, improving upon one-stage primary sample space algorithms, i.e., PSSMLT with Gaussian proposals (PSSMLT / G) and H2MC. One variant of our method first attempts an isotropic Gaussian proposal, resorting to more intricate kernels (that improve local exploration with differential information) only when the first attempt failed, e.g., on rough dielectrics. DRMLT focuses computations in hard-to-explore regions without compromising quality in comparatively simpler regions (e.g., on the board). We visualize a per-pixel relative second-stage acceptance, where violet and yellow extremes respectively indicate the efficiency of the first and second stages."

abstract: |
    Designing robust mutation strategies for primary sample space Metropolis light transport is a challenging problem: poorly-tuned mutations both hinder state space exploration and introduce structural image artifacts. Scenes with complex materials, lighting and geometry make hand-designing strategies that remain optimal over the entire state space infeasible. Moreover, these difficult regions are often sparse in state space, and so relying exclusively on intricate (often expensive) proposal mechanisms can be wasteful where simpler inexpensive mechanisms are more sample efficient. We generalize Metropolis–Hastings light transport to employ a flexible two-stage mutation strategy based on delayed rejection [<a href="https://academic.oup.com/biomet/article-abstract/88/4/1035/2722143">Green & Mira 2001</a>; <a href="https://onlinelibrary.wiley.com/doi/abs/10.1002/%28SICI%291097-0258%2819990915/30%2918%3A17/18%3C2507%3A%3AAID-SIM272%3E3.0.CO%3B2-J">Tierney & Mira 1999</a>]. Our approach generates multiple proposals based on the failure of previous ones, all while preserving Markov chain ergodicity. This allows us to reduce error while maintaining fast global exploration and low correlation across chains. Direct application of delayed rejection to light transport leads to low acceptance probabilities, and so we also propose a novel transition kernel to alleviate this issue. We benchmark our approach on several applications including <i>bold-then-timid</i> and <i>cheap-then-expensive</i> proposals across different light transport algorithms. Our method is applicable to any primary sample space algorithm with minimal implementation effort, producing consistently better results on a variety of challenging scenes.

# video: https://www.youtube.com/embed/k3I17MNou7U

acknowledgements: Computing resources were provided by the <a href="https://www.computecanada.ca/">National Systems of Compute Canada</a>. This research was partially funded by the Natural Sciences and Engineering Council of Canada (RGPIN-2018-05669) and JSPS KAKENHI (18KK0309).

downloads:
    published: false
    paper:
        file: #RiouxLavoie-2020-DRMLT.pdf
        size: #25MB
        file-lowres: #RiouxLavoie-2020-DRMLT-Lowres.pdf
        size-lowres: #3MB
    doi:
        url: #doi
    supplementary:
        file: #DRMLT-Supplemental.zip
        size: #350MB
        url: #supplementary
    slides:
        file: #DRMLT-Presentation.pdf
        size: #30MB
        file-key: #DRMLT-Presentation.key
        size-key: #100MB
    video:
        file: #DRMLT-Video.mp4
        size: #100MB
        url: #video
    code:
        file: #DRMLT-Code.zip
        size: #25MB
        url: #https://github.com/joeylitalien/drmlt
    bibtex:
        file: #DRMLT-BibTeX.bib
        size: #1KB

tex: |
    @article{Rioux-Lavoie:2020:DRMLT,
       author = {Rioux-Lavoie, Damien and Litalien, Joey and Gruson, Adrien and Hachisuka, Toshiya and Nowrouzezahrai, Derek},
       title = {Delayed Rejection {M}etropolis Light Transport},
       journal = {ACM Transactions on Graphics (To be presented at SIGGRAPH 2020)},
       volume = {X},
       number = {XX},
       year = {2020},
       month = jul,
       doi = {XXX}
    }

tag: research
permalink: /publications/drmlt
featured: 1
---