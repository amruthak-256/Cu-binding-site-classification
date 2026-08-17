# Decoding the Structural Diversity of Mononuclear Copper Binding Sites

This repository contains the code, input/output files, and trained models supporting the classification of copper-binding sites described in the article.

## 1. Clustering of copper-binding sites

Hierarchical agglomerative clustering of structural and biochemical features of Cu(I) and Cu(II) binding sites, resulting in a **4+9 subclass classification framework**.

```text
01_clustering/
├── Data/
│   ├── Cu1-ids.csv
│   ├── Cu2-ids.csv
│   ├── input.csv
│   └── output.csv
│
└── code/
    ├── Data_extraction.ipynb
    ├── Featurization.ipynb
    ├── Agglomerative-clustering.ipynb
    ├── Random-subsampling-clustering.ipynb
    ├── Analysis-of-30-clusters.ipynb
    └── Cu1-vs-Cu2-analysis.ipynb

## 2. Prediction of copper-binding site class

Machine-learning classifier for identifying copper-binding site subclasses based on the 9+4 classification framework.

```text
02_classification/
├── Data/
│   ├── binding_sites.xlsx
│   ├── nonredundant_binding_sites_water_fixed.csv
│   ├── final_cluster_classifier.pkl
│   ├── feature_scaler.pkl
│   └── label_mapping.pkl
│
└── Code/
    ├── CD-Hit.ipynb
    └── Classifier.ipynb

## Citation

[Manuscript citation / DOI]
