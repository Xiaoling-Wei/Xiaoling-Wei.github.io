---
title: "ML-Based Recommendation of OTC Treatments and Exercise Modalities for Knee Joint Pain Using Long-Tail Classification"
date: 2025-08-01
reading_time: false
tags:
  - Machine Learning
  - Healthcare AI
  - Long-tail Classification
  - Python
  - TensorFlow
  - LightGBM
---

**Submitted to Expert Systems With Applications (ESWA-D-25-26442)**

**Authors:** Liyuan Gao†, **Xiaoling Wei†**, Tun-Min Jai, Jean-Michel Brismée, Kiran Sagani, Ming-Chien Chyu, Chwan-Li Shen, Victor S. Sheng

†*Co-first authors with equal contribution*

---

Knee osteoarthritis (KOA) is a widespread chronic condition significantly impacting quality of life, particularly for older adults. Although various over-the-counter (OTC) medications and exercise modalities are available for symptom management, patients often struggle to identify effective treatments without personalized guidance.

In this study, we analyzed clinical and demographic data from **1,687 patients** and developed machine learning-based models to assist in making more meaningful treatment recommendations. We addressed the challenge of severe **long-tail label distributions** across 36+ OTC categories and 53+ exercise types using resampling and reweighting strategies.

<!--more-->

## Key Contributions

- Developed ML models to predict individualized OTC treatments and exercise modalities from patient-level clinical and self-reported data.
- Addressed significant class imbalance across 36 OTCs and 53 exercise types using **SMOTE** and class-weighted learning.
- Conducted comprehensive evaluation of four models — Logistic Regression, Random Forest, **LightGBM**, and Focal Loss Neural Network.
- Proposed strategies to incorporate records with missing target labels, reducing reliance on fully labeled data.
- Showed that simple tokenization of textual features slightly outperformed BERT-based embeddings in this structured clinical setting.

## Results

| Task | Model | Accuracy | Macro-F1 |
|------|-------|----------|----------|
| OTC Recommendation | LightGBM + SMOTE | 47.28% | 37.84% |
| Exercise Recommendation | LightGBM + SMOTE | 62.67% | 32.69% |

Results are remarkable given the 36+ OTC categories and 53+ exercise types in a severely imbalanced dataset. LightGBM consistently outperformed all baseline models.

## Tech Stack

Python · TensorFlow · LightGBM · scikit-learn · SMOTE · BERT · Pandas · NumPy
