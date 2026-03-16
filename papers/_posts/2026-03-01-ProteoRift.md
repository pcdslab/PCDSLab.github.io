---
layout: paper
title: "End-to-end deep attention-based multitask pipeline for predicting uncertainty-quantified peptide properties from mass spectrometry data"
nickname: proteorift-paper
authors: "Tariq, Usman; Shabbir, Bilal; Saeed, Fahad;"
year: "2026"
journal: "Nature Scientific Reports"
volume: 
issue:
pages: 
is_published: True
image: /assets/images/papers/nature.png
projects: [ML-MS]
tags: [journal]

# Text
fulltext: https://www.nature.com/articles/s41598-026-43215-2
pdf: 
pdflink:
pmcid:
preprint: 
supplement:

# Links
doi: "10.1038/s41598-026-43215-2"
pmid:

# Data and code
github: [https://github.com/pcdslab/ProteoRift]
neurovault:
openneuro: []
figshare:
figshare_names:
osf:
---
{% include JB/setup %}

# Abstract

Mass-based filtering significantly reduces the peptide candidate pool for subsequent scoring in database search algorithms. While useful, filtering based on one property may lead to exclusion of non-abundant spectra and uncharacterized peptides – potentially exacerbating the streetlight effect. Here we present ProteoRift, a novel attention and multitask deep-network, which can predict multiple peptide properties (length, missed cleavages, and modification status) directly from spectra 77.8% of the time. Integrating ProteoRift into an end-to-end pipeline significantly reduces the search space compared to mass-only filtering. This delivers 8x to 12x speedups while maintaining peptide deduction accuracy comparable to established algorithmic techniques. We also developed uncertainty estimation metrics, which can distinguish between in-distribution and out-of-distribution data (ROC-AUC 0.99) and predict high-scoring mass spectra against the correct peptide (ROC-AUC 0.94). These models and metrics are integrated in an end-to-end pipeline available at https://github.com/pcdslab/ProteoRift.

