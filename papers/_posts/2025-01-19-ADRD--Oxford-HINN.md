---
layout: paper
title: "HINN prioritizes multi-omics biomarkers associated with cognitive decline"
nickname: oxford-ADRD-HINN
authors: "Yashu Vashishath; Sarah Beaver; Saeed, Fahad; Serdar Bozdag;"
year: "2026"
journal: "Oxford Bioinformatics"
volume: 
issue: btag741
pages: 1-12
is_published: True
image: /assets/images/papers/oxford.png
projects: [ML-ADRD]
tags: [ML, gene, ADRD]

# Text
fulltext: https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btag741/8875879?searchresult=1
pdf: https://academic.oup.com/bioinformatics/advance-article-pdf/doi/10.1093/bioinformatics/btag741/71666834/btag741.pdf
pdflink:
pmcid:
preprint: 
supplement:

# Links
doi: 10.1093/bioinformatics/btag741
pmid: PMC11712636

# Data and code
github: 
neurovault:
openneuro: []
figshare:
figshare_names:
osf:
---
{% include JB/setup %}

# Abstract
Integrating multi-omics data for disease prediction remains challenging due to the complexity of cross-layer biological interactions and the limited use of prior biological knowledge in many machine learning models. We present the Hierarchical Input Neural Network (HINN), a deep learning framework that incorporates biologically informed connections across genomic, epigenetic, and transcriptomic layers to model regulatory relationships in a structured and interpretable manner. HINN was applied to blood-derived multi-omics data to predict cognitive assessment scores, including MMSE, MoCA, ADAS11, and RAVLT.Immediate. A biologically guided feature construction pipeline was used to integrate GWAS-derived SNPs, promoter-region DNA methylation, and gene expression data through Gene Ontology Biological Process (GO-BP) and KEGG pathway mappings.

# Results
The model was evaluated using a rigorous training strategy that separates feature selection from testing and incorporates cross-validation as well as repeated runs to ensure robustness. Across all cognitive outcomes, HINN achieved the lowest mean normalized MSE among the evaluated models, with statistically significant improvements over most baseline methods. Ablation analyses showed that the contributions of individual omics modalities and biologically informed connectivity varied across cognitive outcomes, with the clearest benefits of structured connectivity observed for ADAS11 and MMSE. Feature attribution analysis identified a multi-omics cascade involving SNP (rs116557230), CpG site (cg24041822), and a SOCS4 gene expression probe, which showed consistent associations with multiple cognitive outcomes. These findings highlight the ability of HINN to uncover biologically meaningful cross-omics relationships relevant to cognitive decline. Together, this work demonstrates that integrating deep learning with biological knowledge enables biomarker discovery for complex diseases.
