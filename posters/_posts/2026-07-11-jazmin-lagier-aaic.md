---
layout: paper
title: "Interpretable Graph Neural Network Integration of Multimodal Biomarkers for Alzheimer’s Disease Classification"
nickname: aaic-gat-ad-2026
authors: "Jazmin Lagier; Fahad Saeed"
year: "2026"
conference: "AAIC-2026"
image: /assets/images/posters/AAIC-2026-Jazmin-Lagier.png
projects: ["AD-GNN"]
tags: []

# Content
# fulltext: https://alz.confex.com/alz/2024/meetingapp.cgi/Paper/89944
pdf: 

# Links
doi: 


# Data and code
github:
neurovault:
openneuro:
figshare:
figshare_names:
osf:
f1000:
---

{% include JB/setup %}

# Introduction
Alzheimer’s disease (AD) is characterized by the progressive effects of protein pathology, regional neurodegeneration, and network-level functional disruption across the brain. Multimodal neuroimaging captures complementary disease aspects: positron emission tomography (PET) quantifies molecular burden, structural magnetic resonance imaging (sMRI) measures regional atrophy, and functional MRI (fMRI) reveals connectivity alterations [1]. While evidence shows that integrating multiple data modalities may result in improved diagnostic performance, most existing approaches combine biomarkers within black-box frameworks with limited explainability. Objective: Develop an interpretable graph-based framework that integrates multimodal biomarkers to classify cognitively normal (CN) vs. Alzheimer’s disease (AD) and to identify the brain regions and biomarkers that drive predictions.

# Methods
## Graph construction

Each brain was modeled as a graph \(G = (V, E, X)\), where each node corresponds to one of 112 brain regions defined by the Desikan–Killiany atlas. Functional connectivity derived from resting-state fMRI was used to construct the weighted adjacency matrix using Fisher Z-transformed Pearson correlation coefficients between regional time series.

Each node contained a 19-dimensional multimodal feature vector integrating demographic variables, APOE genotype, PET-derived pathology indicators, and sMRI measures. This graph representation allowed the model to jointly learn regional biological attributes and large-scale network interactions associated with AD.

## Model architecture

The graph convolutional network (GCN) architecture consisted of three graph convolutional layers with hidden dimensions of 160, 160, and 80. Each layer was followed by batch normalization, ReLU activation, and dropout. Subject-level graph embeddings were generated using global mean pooling, with seven-network pooling used to derive network-level representations, followed by a final linear classification head for CN versus AD prediction.

## Interpretability framework

Model interpretability was assessed using Integrated Gradients (IG) to quantify feature-level contributions to the prediction. Regional attribution scores were obtained by aggregating feature attributions within each brain region of interest. In addition, feature-set ablation was performed to estimate modality-specific contributions by measuring performance changes after removing multimodal feature groups.


# Results
The full multimodal model achieved the strongest classification performance, with an AUC of 0.94 ± 0.04, balanced accuracy of 0.87 ± 0.05, F1-score of 0.73 ± 0.09, sensitivity of 0.82 ± 0.12, and specificity of 0.92 ± 0.06.

Compared with reduced models, performance was substantially improved over the baseline model (AUC 0.63 ± 0.04), the +PET model (AUC 0.83 ± 0.09), and the +sMRI model (AUC 0.82 ± 0.09), demonstrating the value of integrating multimodal biomarkers with functional connectivity representations.

Modality contribution analysis showed that sMRI and fMRI contributed the most to classification performance, while PET biomarkers further improved diagnostic sensitivity and overall performance. Approximate modality contributions were: sMRI 28.1%, fMRI 24.0%, amyloid PET 17.6%, tau PET 15.9%, demographics 14.3%, and APOE 0.1%.

Integrated-gradient regional attribution analysis identified highly contributing regions including the hippocampus, entorhinal cortex, posterior cingulate cortex, inferior parietal cortex, fusiform cortex, amygdala, temporal pole, lateral orbitofrontal cortex, and supramarginal gyrus. These findings are consistent with known Alzheimer’s disease neurodegenerative pathways and default mode network disruption.


# Conclusions
This work presents an interpretable multimodal graph neural network framework for Alzheimer’s disease classification. Integrating fMRI-derived graph topology with demographic, genetic, PET, and sMRI biomarkers produced the best overall classification performance.  The results support the complementary role of structural neurodegeneration, molecular pathology, and network-level dysfunction in AD representation learning. Importantly, the interpretability analysis recovered biologically meaningful brain regions associated with Alzheimer’s disease, showing that the framework can provide both strong predictive performance and clinically relevant insight into the regional basis of classification.
