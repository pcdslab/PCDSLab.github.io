---
layout: paper
title: "A Machine Learning and Benchmarking Approach for Molecular Formula Assignment of Ultra High-Resolution Mass Spectrometry Data from Complex Mixtures"
nickname: dom-formula-assignment-paper
authors: "Shabbir, Bilal; Oliveira, Pablo R B; Fernandez-Lima, Francisco; Saeed, Fahad;"
year: "2026"
journal: 
volume: 
issue: 
pages: 
is_published: False
image: /assets/images/papers/biorxiv.png
projects: [ML-MS]
tags: [preprint]

# Text
fulltext: https://www.biorxiv.org/content/10.64898/2026.02.17.706479v1
pdf:
pdflink: https://www.biorxiv.org/content/10.64898/2026.02.17.706479v1.full.pdf
pmcid:
preprint:  
supplement:

# Links
doi: https://doi.org/10.64898/2026.02.17.706479
pmid:

# Data and code
github: [https://github.com/pcdslab/dom-formula-assignment-using-ml]
neurovault:
openneuro: []
figshare:
figshare_names:
osf: []
---
{% include JB/setup %}

# Abstract

A machine learning approach to molecular formula assignment is crucial for unlocking the full potential of ultra-high resolution mass spectrometry (UHRMS) when analyzing complex mixtures. By combining data-driven models with rigorous benchmarking, the accuracy, consistency, and speed in identifying plausible molecular formulas from vast spectral datasets can be improved. Compared with traditional de novo methods that rely heavily on rule-based heuristics, and manual parameter tuning, machine learning approaches can capture complex patterns in data and adapt more readily to diverse sample types. In this paper, we describe the application of a machine learning methods using the k-nearest neighbors (KNN) algorithm trained on curated chemical formula datasets of UHRMS analysis of dissolved organic matter (DOM) covering the saline river continuum and tropical wet/dry season variability. The influence of the mass accuracy (training set with 0.15-1ppm) was evaluated on a blind test set of DOMs of different geographical origins. A Decision Tree Regressor (DTR) and Random Forest Regressor (RFR) based on mass accuracy (<1ppm) was used. Results from our ML models exhibit 43% more formulas annotated than traditional methods (5796 vs 4047), Model-Synthetic achieved 99.9% assignment rate and annotated/assigned 2x more formulas (8,268 vs 4047). DTR and RFR achieved formula-level accuracies (FA) of 86.5% and 60.4%, respectively. Overall, results show an increase in formula assignment when compared with traditional methods. This ultimately enables more reliable characterization of complex natural and engineered systems, supporting advances in fields such as environmental science, metabolomics, and petroleomics. Furthermore, the novel data set produced for this study is made publicly available, establishing an initial benchmark for molecular formula assignment in UHRMS using machine learning. The dataset and code are publicly available at: https://github.com/pcdslab/dom-formula-assignment-using-ml.