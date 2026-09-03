---
layout: paper
title: "ProtEnrich: Residual Multimodal Enrichment of Protein Sequence Embeddings"
nickname: ProtEnrich-paper
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
pdf: https://www.biorxiv.org/content/10.64898/2026.08.24.746797v1.full.pdf
pdflink: 
pmcid:
preprint:  https://www.biorxiv.org/content/10.64898/2026.08.24.746797v1.full
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
Protein language models effectively capture evolutionary and functional signals from sequence data but lack explicit representation of the biophysical properties that govern protein structure and dynamics. Existing multimodal approaches attempt to integrate such physical information through direct fusion, often requiring multimodal inputs at inference time and distorting the geometry of the sequence embedding space, which can disrupt the semantic organization learned from evolutionary information. Consequently, a fundamental challenge of how to incorporate structural and dynamical knowledge into sequence representations without disrupting their semantic organization, enabling sequence-based models to better capture the biophysical properties governing protein structure and function. We introduce ProtEnrich, a representation learning framework based on a residual multimodal enrichment paradigm. Pro-tEnrich decomposes sequence embeddings into two complementary latent subspaces, an anchor subspace that preserves sequence semantics, and an alignment subspace that encodes biophysical relationships. By converting multimodal information derived from ProstT5 and RocketSHP to a low-energy residual component, our approach injects physical representation while maintaining the original sequence embedding while preserving their original semantic geometry, avoiding the need for multimodal inputs at inference time. Across eight diverse protein foundational models trained on 550,120 SwissProt proteins with AlphaFold structures, enriched embeddings improved zero-shot remote homology retrieval, increasing Precision@10 and MRR by up to 0.13 and 0.11, respectively. Downstream performance also improved on structure-dependent tasks, reducing fluorescence prediction error by up to 16% and increasing metal ion binding AUCROC by up to 2.4 points, while requiring only sequence input at inference. Source code is available at https://github.com/pcdslab/ProtEnrich, pretrained models and datasets are available at https://huggingface.co/collections/SaeedLab/protenrich.