---
title: "Balancing Accuracy and Efficiency in UAV Intrusion Detection: A Leakage-Aware Multi-Dataset Study"
date: 2026-01-01
reading_time: false
tags:
  - UAV Security
  - Intrusion Detection
  - Machine Learning
  - Deep Learning
  - Python
  - PyTorch
links:
  - icon: fab fa-github
    icon_pack: fab
    name: Code
    url: https://github.com/SESAIS/2026-MultiDatasets-CNN-RF--SVC
---

**Authors:** Noah Deri Ogilvie, **Xiaoling Wei**, Damiano Torre

---

The increasing adoption of unmanned aerial vehicles (UAVs) in civilian and defense applications introduces critical cybersecurity challenges, particularly in resource-constrained environments where intrusion detection systems (IDS) must balance accuracy and efficiency. This work investigates machine learning and deep learning approaches for UAV-specific intrusion detection, focusing on a hybrid Random Forest–Support Vector Classifier (RF–SVC) and a one-dimensional Convolutional Neural Network (1D-CNN).

A key contribution of this study is the adoption of a **group-aware evaluation strategy** that preserves temporal and contextual dependencies across UAV flight sessions. This approach prevents data leakage and mitigates the optimistic bias introduced by conventional stratified sampling, enabling a more reliable and realistic assessment of model generalization.

<!--more-->

## Key Contributions

- **C1:** First unified, leakage-aware preprocessing and evaluation pipeline applied across four diverse public UAV datasets (UAV-Attack, T-ITS, UAVCAN Attack, ISOT-Drone).
- **C2:** Design and evaluation of two complementary architectures — a hybrid RF–SVC and a 1D-CNN — analyzing both detection performance and inference latency for real-time UAV intrusion detection.
- **C3:** Demonstrated that group-aware evaluation yields more conservative and realistic estimates of model generalization compared to conventional stratified splitting.
- **C4:** Released a complete open-source artifact including preprocessing pipelines, model implementations, and evaluation scripts.

## Results

| Dataset | Model | Accuracy | F1-Score |
|---------|-------|----------|----------|
| ISOT-Drone | 1D-CNN | 99.74% | 93.86% |
| T-ITS | 1D-CNN | 87.83% | 88.97% |
| UAV Attack | RF-SVC | 96.45% | 95.56% |
| UAVCAN-Attack | 1D-CNN | 97.41% | 96.61% |

The 1D-CNN achieves superior detection capability in complex sequential scenarios, while the RF–SVC provides a more efficient alternative with competitive performance.

## Tech Stack

Python · PyTorch · scikit-learn · XGBoost · RAPIDS cuML · Random Forest · SVM · 1D-CNN
