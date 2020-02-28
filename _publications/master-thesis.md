---
layout: pub

short-title: LVRS
title: Learning Visibility in Ray Space
authors:
    - author: 
        name: Joey Litalien
        institution: McGill University
        link: https://joeylitalien.github.io

journal: Master's thesis
journal-note: M.Eng.
volume: 
number: 
month: December
year: 2018

thumbnail: /assets/thumbnails/mthesis-thumb.png
teaser: /assets/teasers/mthesis-teaser.png
teaser-caption: 

abstract: >
    Soft shadows from area lights are essential in generating compelling photorealistic images but require tracing secondary rays to evaluate visibility for direct lighting. This computation is costly and, as such, is usually replaced by image- or geometry-based approximations for real-time rendering. In this work, we investigate the use of deep learning techniques to solve the visibility problem. By treating occlusion as a binary classification task, we train a per-object artificial neural network that estimates the directional visibility profile in ray space. We test on low-tomoderate complexity meshes with different light sources and show that a simple feedforward neural network classifier is partially capable of generalizing to unseen light positions. Unfortunately, our model has difficulties reconstructing shadows past a certain distance and cannot accurately resolve shadows in all directions.


downloads:
    paper:
        file: 
        size: 
    bibtex:
        file: 
        size:

tex: |
    @masterthesis{Litalien:2019:LVRS,
       author = {Litalien, Joey},
       title = {Learning Visibility in {R}ay {S}pace},
       schol = {McGill University}
       year = {2018},
       month = dec
    }

tag: research
permalink: /publications/masterthesis
featured: 2
---