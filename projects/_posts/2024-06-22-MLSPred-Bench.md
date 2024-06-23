---
layout: project
title: "MLSPred-Bench: Reference EEG Benchmark for Prediction of Epileptic Seizures"
contributors: [Prof-S,umairmy305]
handle: MLSPred-Bench
status: collection
type: dataset

# Optional
website: 
grant: NSF TT-2213951
grant_url: https://www.nsf.gov/awardsearch/showAward?AWD_ID=2213951&HistoricalAwards=false
image: /assets/images/projects/2024-06-22-raw-EEG-signal.png
tagline: '"Reference EEG Benchmark for Prediction of Epileptic Seizures"'
tags: [eeg]

# Data and code
github: https://github.com/pcdslab/MLSPred-Bench
neurovault:
openneuro:
figshare:
figshare_names:
osf:
---
{% include JB/setup %}

MLSPred-Bench will create 12 different benchmarks based on different values of the seizure prediction horizon (SPH) and the seizure occurrence period (SOP). The benchmarks are for patient-independent epileptic seizure prediction using only raw electroencephalography (EEG) data and are machine learning (ML)-ready.

For each benchmark, MLSPred-Bench draws preictal segments of length from the SPH duration. We assume there is a gap equal to the SOP in minutes before the start of a seizure where the SPH ends. The datasets are class-balanced where an equal amount of interictal samples are drawn from sessions of the same subject where there were no seizures. 


## Participate

Data collection and curation for this study is complete.
