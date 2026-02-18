---
layout: paper
title: "MolDeBERTa: Foundational Model for Physicochemical and Structural-Informed Molecular Representation Learning"
nickname: MolDeBERTa-paper
authors: "Oliveira, Gabriel Bianchin; Saeed, Fahad;"
year: "2026"
journal: 
volume: 
issue: 
pages: 
is_published: False
image: /assets/images/papers/biorxiv.png
projects: [ML-molecular-protein-representation]
tags: [molecules]

# Text
fulltext: https://www.biorxiv.org/content/10.64898/2026.02.15.706011v1
pdf:
pdflink: https://www.biorxiv.org/content/10.64898/2026.02.15.706011v1.full.pdf
pmcid:
preprint:  
supplement:

# Links
doi: https://doi.org/10.64898/2026.02.15.706011 
pmid:

# Data and code
github: [https://github.com/pcdslab/MolDeBERTa]
neurovault:
openneuro: []
figshare:
figshare_names:
osf: []
---
{% include JB/setup %}

# Abstract

Foundational models that learn the language of molecules are essential for accelerating the material and drug discovery. These self-learning models can be trained on a large number of unlabelled molecules, enabling applications like property prediction, molecule de-sign (de novo generation, optimization), and screening for specific functions. However, existing molecular language models are built upon first-generation transformer architectures and are pretrained using masked language modeling, a generic token-level objective that is agnostic to physicochemical and structural molecular properties. Here we introduce MolDe-BERTa, a structure-informed self-supervised molecular encoder that leverages a byte-level Byte-Pair Encoding (BPE) tokenization strategy. MolDeBERTa is pretrained on up to 123 million SMILES molecules from PubChem, representing one of the largest publicly available SMILES-based corpora. To achieve this, we introduce three novel pretraining objectives designed to inject strong inductive biases for molecular properties and structural similarity directly into the latent space, resulting in reduced gap between linguistic chemical representations and physical molecular properties. The model was then systematically investigated across three architectural scales, two dataset sizes, and five distinct pretraining objectives. MolDeBERTa when evaluated on 9 downstream MoleculeNet benchmarks outperformed existing masked language models, achieving up to a 16% reduction in regression error and improvements of up to 3.0 ROC-AUC points on classification benchmarks. MolDeBERTa advances unsupervised encoder-based foundational models at scale both for pretraining data and downstream evaluation, enabling data-efficient chemistry-informed representation learning. The source code is publicly available at https://github.com/pcdslab/MolDeBERTa, and Hugging Face at https://huggingface.co/collections/SaeedLab/moldeberta. All the pretraining datasets are available at https://huggingface.co/datasets/SaeedLab/MolDeBERTa. 