---
layout: paper
title: "fairGNN-WOD: fair graph learning without demographics"
nickname: fairGNN-colab-paper
authors: "Zichong Wang; Fang Liu; Shimei Pan; Jun Liu; Fahad Saeed; Meikang Qiu; Wenbin Zhang;"
year: "2025"
journal: "IJCAI '25: Proceedings of the Thirty-Fourth International Joint Conference on Artificial Intelligence"
volume: 
issue: Article 63
pages: 556 - 564
is_published: True
image: /assets/images/papers/acm.jpg
projects: [ML-brain-imaging]
tags: [ML, ASD, ADRD, Multisite]

# Text
fulltext: 
pdf:
pdflink: https://www.ijcai.org/proceedings/2025/0063.pdf
pmcid:
preprint:  
supplement:

# Links
doi: 10.24963/ijcai.2025/63
pmid:

# Data and code
github: []
neurovault:
openneuro: []
figshare:
figshare_names:
osf: []
---
{% include JB/setup %}

# Abstract

Graph Neural Networks (GNNs) have excelled in diverse applications due to their outstanding predictive performance, yet they often overlook fairness considerations, prompting numerous recent efforts to address this societal concern. However, most fair GNNs assume complete demographics by design, which is impractical in most real-world socially sensitive applications due to privacy, legal, or regulatory restrictions. For example, the Consumer Financial Protection Bureau (CFPB) mandates that creditors ensure fairness without requesting or collecting information about an applicant's race, religion, nationality, sex, or other demographics. To this end, this paper proposes fairGNN-WOD, a first-of-its-kind framework that considers mitigating unfairness in graph learning without using demographic information. In addition, this paper provides a theoretical perspective on analyzing bias in node representations and establishes the relationship between utility and fairness objectives. Experiments on three real-world graph datasets illustrate that fairGNN-WOD outperforms state-of-the-art baselines in achieving fairness but also maintains comparable prediction performance.