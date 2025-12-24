# Customer Segmentation Using Unsupervised Learning

## Overview
This project applies unsupervised machine learning techniques to identify actionable customer segments from retail transaction data. The work is structured as an open-source style data science project with reproducible code and documented artifacts.

## Problem Type
Unsupervised Learning – Clustering

## Dataset
Superstore Sales Dataset (Kaggle)

## Methods
- Customer-level feature aggregation
- Feature scaling and winsorization
- PCA (93% explained variance)
- K-Means, Agglomerative Clustering, DBSCAN
- Internal validation and stability analysis
- Surrogate model explainability
- Fairness and bias auditing

## Final Model
K-Means (k = 2)

## Repository Structure

```text
capstone-project/
│
├── data/
│   ├── raw/
│   │   └── superstore_final_dataset.xlsx
│   └── processed/    
│       ├── customer_features_with_provisional_clusters.xlsx
│       ├── data_dictionary.xlsx
│       ├── surrogate_feature_importance.xlsx
│       ├── X_pca.xlsx
│       └── X_preprocessed_selected
│
├── arrays
│       ├── labels/
│       │   ├── agg_labels_k2.npy
│       │   ├── dbscan_labels_eps1.5_ms10.npy
│       │   └── kmeans_labels_k2.npy
│       ├── config/
│       │   ├── agg_config_k2.json
│       │   ├── dbscan_config_eps1.5_ms10.json
│       │   └── kmeans_config_k2.json
│       └── eval/    
│           ├── agg_eval_k2.json
│           ├── dbscan_eval_eps1.5_ms10.json
│           └── kmeans_eval_k2.json
│
├── models/
│   └── kmeans_model_k2.joblib
│
├── metrics/
│       ├── agg_tuning_metrics.xlsx
│       ├── dbscan_tuning_metrics.xlsx
│       ├── kmeans_tuning_metrics.xlsx
│       └── model_comparison_summary.xlsx
│       
├── notebooks/
│   ├── 1. Fangonilo_Franz_Capstone Project Python Script.ipynb
│   └── 2. Fangonilo_Franz_Capstone Project Technical Deck.ipynb
│
│
├── docs/
│   ├── Fangonilo_Franz_Capstone Project Business Deck.pdf
│   └── Fangonilo_Franz_Capstone Project Write-up.docx
│
└── README.md              
```

## Reproducibility
1. Install dependencies:
```bash
pip install -r requirements.txt
```
2. Run notebooks in numerical order.

Final Report

The full written report is available in docs/Fangonilo_Franz_Capstone Project Write-up.docx.


---

# ✅ 5️⃣ requirements.txt (Rubric Pass)

Minimal and sufficient:

```txt
numpy
pandas
scikit-learn
scipy
matplotlib
seaborn
jupyter
```
