---
layout: project
title: ASD-AE-Harmonization
contributors: [Prof-S, falmuqhim]
handle: AE-fMRI-Harmonization
status: complete


# Optional
website: 
grant:
grant_url:
image: /assets/images/software/open-source.png
tagline: Autoencoder-based harmonization of multisite fMRI for robust autism classification
tags: [software]

# Data and code
github: https://github.com/pcdslab/Autoencoder-fMRI-Harmonization
neurovault:
openneuro:
figshare:
figshare_names:
osf: https://osf.io/d8253
---
{% include JB/setup %}

We propose an autoencoder-based framework for harmonizing multisite functional magnetic resonance imaging (fMRI) data to improve the generalizability of machine learning models across imaging centers. Our approach leverages the non-linear representation learning capability of autoencoders to reduce site-specific variability while preserving biologically meaningful signal, without relying on additive or multiplicative statistical assumptions. Unlike traditional harmonization methods, our framework avoids data leakage by eliminating the need for access to data from all sites during model training. We design and evaluate multiple autoencoder variants, including AE, SAE, TAE, and DAE, and assess their effectiveness using the Autism Brain Imaging Data Exchange I (ABIDE-I) dataset comprising 1,035 subjects from 17 imaging centers. Experimental results using leave-one-site-out cross-validation demonstrate statistically significant improvements over baseline models (p < 0.01), with mean classification accuracy gains ranging from 3.41% to 5.04%. These findings highlight the effectiveness of autoencoder-based harmonization for reducing site effects, improving robustness on unseen sites, and enabling reliable downstream neuroimaging analyses.

## Status 
The method development for this work is complete