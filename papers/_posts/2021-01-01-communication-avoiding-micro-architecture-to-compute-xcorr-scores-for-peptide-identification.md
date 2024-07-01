---
layout: paper
title: "Communication-avoiding micro-architecture to compute Xcorr scores for peptide identification"
nickname: 2024-04-16-bottenhorn-salo-diva
authors: "Kumar, Sumesh; Saeed, Fahad; "
year: "2021"
journal: IEEE
volume: 
issue:
pages: 99-103
is_published: True
image: /assets/images/papers/biorxiv.png
projects: []
tags: []

# Text
fulltext:
pdf:
pdflink:
pmcid:
preprint: 
supplement:

# Links
doi: "10.1109/FPL53798.2021.00024"
pmid:

# Data and code
github: [""]
neurovault:
openneuro: []
figshare:
figshare_names:
osf:
---
{% include JB/setup %}

# Abstract

Database algorithms play a crucial part in systems biology studies by identifying proteins from mass spectrometry data. Many of these database search algorithms incur huge computational costs by computing similarity scores for each pair of sparse experimental spectrum and candidate theoretical spectrum vectors. Modern MS instrumentation techniques which are capable of generating high-resolution spectrometry data require comparison against an enormous search space, further emphasizing the need of efficient accelerators. Recent research has shown that the overall cost of scoring, and deducing peptides is dominated by the communication costs between different hierarchies of memory and processing units. However, these communication costs are seldom considered in accelerator-based architectures leading to inefficient DRAM accesses, and poor data-utilization due to irregular memory access patterns …
