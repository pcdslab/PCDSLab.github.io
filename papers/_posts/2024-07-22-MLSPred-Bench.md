---
layout: paper
title: "MLSPred-Bench: ML-Ready Benchmark Leveraging Seizure Detection EEG data for Predictive Models"
nickname: MLSPred-Bench-paper
authors: "Mohammad, Umair; Saeed, Fahad; "
year: "2024"
journal: "bioRxiv"
volume: 
issue:
pages: 1-8
is_published: False
image: /assets/images/papers/biorxiv.png
projects: [ML-seizure]
tags: [preprint]

# Text
fulltext: https://www.biorxiv.org/content/10.1101/2024.07.17.604006v1
pdf:
pdflink: https://www.biorxiv.org/content/10.1101/2024.07.17.604006v1.full.pdf
pmcid:
preprint: 
supplement:

# Links
doi: "10.1101/2024.07.17.604006"
pmid:

# Data and code
github: []
neurovault:
openneuro: []
figshare:
figshare_names:
osf:
---
{% include JB/setup %}

# Abstract

Predicting epileptic seizures is a significantly challenging task as compared to detection. While electroen-cephalography (EEG) data annotated for detection is available from multiple repositories, they cannot readily be used for predictive modeling. In this paper, we designed and developed a strategy that can be used for converting any EEG big data annotated for detection into ML-ready data suitable for prediction. The generalizability of our strategy is demonstrated by executing it on Temple University Seizure (TUSZ) corpus which is annotated for seizure detection. This execution results in 12 ML-ready datasets, collectively called MLSPred-Bench benchmark, which constitutes data for training, validating and testing seizure prediction models. Our strategy uses different variations of seizure prediction horizon (SPH) and the seizure occurrence period (SOP) to make more than 150GB of ML-ready data. To illustrate that the generated data can be used for predictive modeling, we executed an ML model on all the benchmarks which resulted in variable performances when compared with the original model and its performance. We expect that our strategy can be used as a general method to transform seizure detection EEG big data into ML-ready datasets useful for seizure prediction.Our code and related materials will be made available at https://github.com/pcdslab/MLSPred-Bench.
