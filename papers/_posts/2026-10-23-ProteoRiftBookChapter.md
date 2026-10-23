---
layout: paper
title: "ProteoRift Protocols: A Deep Learning Filtering Workflow for Peptide Identification in Mass Spectrometry Data"
nickname: ProteoRift-bookchapter
authors: "Shabbir, Bilal; Tariq, Usman; Saeed, Fahad;"
year: "2026"
journal: Springer Methods in Molecular Biology
volume: 3071
issue: 
pages: 
is_published: True
image: /assets/images/papers/springer.png
projects: [ML-MS]
tags: []

# Text
fulltext: https://link.springer.com/protocol/10.1007/978-1-0716-5519-1_15
pdf: 
pdflink: 
pmcid:
preprint: 
supplement:

# Links
doi: 10.1007/978-1-0716-5519-1_15


pmid:

# Data and code
github: [https://github.com/pcdslab/ProteoRift]
huggingface: ["https://huggingface.co/SaeedLab/ProteoRift"]
neurovault:
openneuro: []
figshare:
figshare_names:
osf: []
---
{% include JB/setup %}

# Abstract
Increasing complexity and volume of mass spectrometry (MS) data have presented new challenges and opportunities for peptide identification in shotgun proteomics. Existing database search algorithms reduce the number of potential candidate peptides by using precursor mass filtering. While useful, relying on a single and simple filter may lead to the exclusion of nonabundant spectra and uncharacterized peptides. In this chapter, we present a machine-learning model, called ProteoRift, capable of predicting multiple properties of the peptide (e.g., length, missed cleavages, and modification status) directly from the spectra. Predicting multiple properties helps to apply more targeted filters in the database search and provides up to 12× speedup as compared to mass-only filtering in peptide identification. This chapter describes the general architecture, which is followed by a step-by-step guide for installing and performing database searches using the ProteoRift model. Lastly, we discuss the data preparation and preprocessing steps required for retraining ProteoRift. ProteoRift is an open-source and open-weights model and is available at https://github.com/pcdslab/ProteoRift.
