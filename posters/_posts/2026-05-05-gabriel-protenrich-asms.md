---
layout: paper
title: "Sequence-Based Enrichment of Structural and Dynamical Protein Representations for Large-Scale Proteomics"
nickname: asms-massspectrometry-2025-poster
authors: "Gabriel Bianchin de Oliveira; Fahad Saeed"
year: "2026"
conference: "ASMS-2026"
image: /assets/images/posters/ProtEnrich-ASMS-2026-poster.png
projects: ["ML-molecular-protein-representation"]
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
Structure and dynamics play a central role in protein function, interaction, and regulation. In mass spectrometry-based proteomics, experiments generate large protein lists, resulting in downstream analyses limited to sequence-level annotations and pathway analysis. Although recent computational approaches have improved structure prediction accuracy, they remain costly, incomplete, and impractical for high-throughput proteomics analyses. Accessing protein dynamics at scale is even more challenging, due to molecular simulations complexity and lack of reliable structural models. Here, we introduce a sequence-based representation learning framework that enriches protein embeddings with latent structural and dynamical information, requiring only sequence at inference time. Our approach leverages sequence-level data (expected from MS based experiments) to extract structural and dynamic insights, bypassing the need for traditional template-based modeling or computationally expensive molecular dynamics simulations.

# Methods
The method uses amino acid sequence as an anchor representation and learns to inject latent structural and dynamical information through supervised and contrastive learning objectives. During training, sequence-based protein representations are aligned with complementary representations derived from structural and dynamical descriptors, enabling the model to associate sequence patterns with biophysical context. Structural and dynamical information is used exclusively during training as residual information. At inference time, enriched protein representations are generated from sequence alone, without requiring explicit structural models, molecular simulations, or multimodal inputs. These sequence-derived enriched embeddings are directly applied to downstream analyses of proteins identified in mass spectrometry-based proteomics workflows.


# Results
We evaluated the proposed sequence enriched protein embeddings on proteins held out from training to assess their ability to recover structural, dynamical, and functional signals without explicit structural input. First, we present that the generated representations closely match reference structural and dynamical representations, achieving average cosine similarities of 0.95 and 0.99, respectively, and providing substantially more informative representations than random baselines. In retrieval experiments, enriched embeddings consistently outperform sequence-only representations. Specifically, we observe improvements of 8.5% in accuracy for remote homology detection at the fold level, 9.7% at the superfamily level, and 10.6% at the family level, indicating improved geometric alignment with underlying biophysical properties. We also assess whether the enriched embeddings recover biologically meaningful functional signals. We show that the representations capture part of the functional information typically associated with explicit structural or dynamical features, despite requiring only sequence at inference time. In standard benchmarks used in the literature, the enriched embeddings improve performance over sequence-only baselines for metal ion binding, protein-protein interaction, and fluorescence prediction tasks by approximately 1.4, 0.5, and 5.3 percentage points, respectively. Together, these preliminary results demonstrate that sequence-based enrichment provides a practical mechanism to incorporate latent structural and dynamical context into downstream analysis of proteins identified in mass spectrometry-based proteomics, enabling structure and dynamics-aware interpretation at proteome scale.


# Conclusions
Enables structure and dynamics-aware analysis of mass spectrometry-identified proteins using only sequence, without structural models or molecular simulations.