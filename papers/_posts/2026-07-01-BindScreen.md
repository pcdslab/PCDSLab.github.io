---
layout: paper
title: "BindScreen: Protein-Centric Contrastive Learning for Sequence-Based Virtual Screening"
nickname: bindscreen-paper
authors: "Oliveira, Gabriel Bianchin; Saeed, Fahad;"
year: "2026"
journal: BioArxiv
volume: 
issue: 
pages: 
is_published: False
image: /assets/images/papers/biorxiv.png
projects: [ML-molecular-protein-representation]
tags: [preprint]

# Text
fulltext: 
pdf: https://www.biorxiv.org/content/10.64898/2026.08.24.746801v1.full.pdf
pdflink: 
pmcid:
preprint:  https://www.biorxiv.org/content/10.64898/2026.08.24.746801v1.full
supplement:

# Links
doi: 
pmid:

# Data and code
github: [https://github.com/pcdslab/ProtEnrich]
huggingface: [https://huggingface.co/collections/SaeedLab/protenrich] 
neurovault:
openneuro: []
figshare:
figshare_names:
osf: []
---
{% include JB/setup %}

# Abstract
Virtual screening ranks candidate molecules against a protein target. Sequence-based deep learning avoids docking’s structural requirements, but pair-based models need one forward pass per protein-molecule pair and scale poorly to large libraries. Dual-encoder contrastive models remove that bottleneck, yet standard CLIP training assumes a symmetric, one-to-one correspondence, whereas protein–molecule binding is asymmetric and many-to-many. We present Bind-Screen, a sequence-only dual-encoder screening model, and show that the decisive design choice is not the contrastive loss but how the batch is built. BindScreen combines a protein-centric batch construction and an asymmetric multi-positive InfoNCE loss. A factorial ablation separates the two contributions: the loss alone degrades performance under standard CLIP batching, the protein-centric batch alone recovers most of the gain, and the combination performs best. The effect is encoder-agnostic across eight protein language models spanning four architectural families. By decoupling protein count from molecule count per batch, BindScreen reaches higher validation BEDROC in 86 hours than standard CLIP reaches in 460 hours, and needs about seven times fewer forward passes to screen LIT-PCBA than pair-based models. The source code, pretrained checkpoints, and datasets are publicly available at https://github.com/pcdslab/BindScreen and https://huggingface.co/collections/SaeedLab/bindscreen.

