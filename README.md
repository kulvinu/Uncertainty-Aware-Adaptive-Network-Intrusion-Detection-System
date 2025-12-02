# Uncertainty-Aware Adaptive Network Intrusion Detection System 🛡️
## Overview

This repository implements an adaptive network intrusion detection system (NIDS) that leverages uncertainty-aware methods together with hybrid meta-learning and multi-agent reinforcement learning (MARL). Its goal is to provide robust, adaptive detection capabilities under dynamic network conditions and evolving threats.

## Description 📝
### What the Code Does

* Implements preprocessing pipelines for network intrusion detection datasets (e.g. CICIDS2017, CICIDS2018), including feature extraction and dataset normalization.

* Builds and trains adaptive NIDS models that incorporate uncertainty estimation when classifying network events.

* Supports evaluation across multiple datasets to assess cross-dataset generalization and robustness.

* Logs training history and outputs performance reports (e.g. detection accuracy, false positives, uncertainty statistics).

### Why “Uncertainty-Aware & Adaptive”

Traditional intrusion detection systems especially signature-based ones, may fail to detect novel or evolving attacks. An anomaly-based approach augmented with uncertainty estimation enables the system to identify suspicious-but-ambiguous events and flag them for further inspection rather than making overconfident predictions.

Using adaptive learning mechanisms (meta-learning / MARL) further allows the model to adjust to shifting traffic patterns, new attack types, and changing normal behaviour over time.

## Features 🌟

* Preprocessing pipelines for datasets (CICIDS2017, CICIDS2018) covering data cleaning, normalization, feature engineering.

* Adaptive detection model integrating uncertainty estimation in decision-making, improving robustness to unknown/novel attacks.

* Cross-dataset evaluation: measure generalization performance across different network environments.

* Training history & reporting: detailed logs and JSON reports (e.g. cross_dataset_report.json, enhanced_adversarial_nids_report.json, etc.).


## Files Included 📂
```
Uncertainty-Aware-Adaptive-Network-Intrusion-Detection-System/
│
├── CICIDS2017_Preprocessing.ipynb
├── CICIDS2018_Preprocessing.ipynb
├── NIDS_System_Implementation.ipynb
├── Benchmark_comparisons.ipynb
│
├── cross_dataset_report.json
├── enhanced_adversarial_nids_report.json
├── enhanced_adversarial_nids_training_history.json
├── enhanced_statistical_adversarial_nids_report.json
│
├── LICENSE
└── README.md
```
## Getting Started 🚀
### Requirements

* Python (>= 3.7) or a suitable version compatible with used libraries.

* Standard data science / ML libraries (Pandas, Numpy, Matplotlib, torch, sklearn)

* Jupyter Notebook (or JupyterLab) to run preprocessing & implementation notebooks.

### Steps to Run

* Clone the repository:
````
git clone https://github.com/kulvinu/Uncertainty-Aware-Adaptive-Network-Intrusion-Detection-System.git
````

* Install any required dependencies.

* Preprocess the datasets by running CICIDS2017_Preprocessing.ipynb and CICIDS2018_Preprocessing.ipynb.

* Open NIDS_System_Implementation.ipynb to train and evaluate the adaptive NIDS model.

* (Optional) Run Benchmark_comparisons.ipynb to compare different configurations or baselines.

* Review output reports (*.json) to analyse performance, generalization, detection rates, and uncertainty metrics.

## Outputs & Reporting 📊

Detection performance metrics (accuracy, precision, recall, false positive / false negative rates).

Uncertainty-aware indicators - enabling more conservative decisions when model confidence is low.

Cross-dataset generalization results - showing how well the model transfers to unseen environments.

Training history and logs to reproduce experiments or audit past runs.

## License ⚖️

This project is licensed under the MIT License. If you copy, modify, distribute, or use the software (or any part of it), the license terms apply.

## Contact / Contribution 💬

For inquiries, please contacct:

Kulanika Gnanaratna
