---
layout: paper
title: "Addressing Fulvic Acids Chemical diversity and structural complexity with High Resolution Trapped Ion Mobility, FT-ICR Mass Spectrometry and Machine Learning"
nickname: asms-massspectrometry-2026-poster-pablo
authors: "Pablo R. B. Oliveira; Bilal Shabbir; Kevin J. Dit Fouque; Chad Weisbrod; David D. Stranz; Anton N. Kozhinov; Konstantin O. Nagornov; Yury O. Tsybin; Fahad Saeed; and Francisco A. Fernandez-Lima"
year: "2026"
conference: "ASMS-2026"
image: /assets/images/posters/Poster_DOM_ASMS_2026.png
projects: ["ML-MS"]
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
The molecular composition and dynamics of dissolved organic matter (DOM) are directly related to the global carbon cycle and ecological dynamics. DOM analysis remains challenging due to the high molecular diversity and complexity, especially at the molecular and structural level. Difficulties associated with isolating, detecting, identifying individual components, and outlining transformation pathways further complicate this effort. There is a need to develop comprehensive and complementary analytical approaches that can reveal the structural signature of DOM in various environments. In this study, we introduce an alternative approach based on the use of machine learning (ML) for the molecular assignment of high-resolution mobility and ultrahigh resolution mass spectrometry data.

# Methods
The rule-based de novo formula assignment algorithm begins by sorting unassigned peaks from high to low abundance, then performs multi-pass de novo formula assignment based on elemental groups (CcHh, CcHhOo, CcHhOoNn, etc.), applying constraints such as a de novo m/z limit, m/z error, minimum abundance, and elemental ratio ranges (H/C, N/C, O/C, P/C, and S/C). Once a candidate formula is identified, a DBE × C map is searched to find monoisotopic peaks differing by CH₂, H2, or O units. Peaks assigned based on their isotopic pattern are then removed from the search list. In contrast, the machine learning approach trains a model on a labeled dataset containing m/z and intensity (Int) values along with known formulas (CcHhOoNn), then applies that trained model to a test set of m/z and intensity data during the prediction process, with final outputs filtered by m/z error and minimum abundance thresholds.


# Results
ML formula assignment reproduced the main chemical space captured by de novo workflows while remaining constrained by the training-set domain. Across SRFA2, SRHA, and SRNOM, ML preserved the dominant oxygen-number distributions, heteroatom-class patterns, and Van Krevelen regions, especially for CHO and CHON formulas. Differences between ML and de novo assignments were strongly influenced by spectral processing, with aFTk and aFTsk improving peak separation and supporting broader formula recovery relative to mFTk. The overlap analysis indicates that missing or unique formulas are mainly driven by resolution, calibration, and training-set coverage rather than random assignment behavior. 


# Conclusions
Together, these results show that ML provides a fast and chemically consistent strategy for DOM formula prediction, but robust performance requires representative training data and validation against ultrahigh resolution de novo assignments.