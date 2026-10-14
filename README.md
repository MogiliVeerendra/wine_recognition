# Wine Clustering Using Machine Learning

## Project Overview

This project uses unsupervised machine learning to group wines based on their chemical properties.

The Wine dataset contains 178 wine samples and 13 numerical features. The goal is to identify groups of wines with similar characteristics without using the original class labels during model training.

Two clustering algorithms are implemented:
- K-Means Clustering
- Hierarchical Clustering

The models are evaluated and compared to understand which algorithm produces better-separated clusters.

## Objectives

- Understand and apply unsupervised learning.
- Explore and preprocess the Wine dataset.
- Scale numerical features before clustering.
- Implement K-Means and Hierarchical Clustering.
- Select the number of clusters using the Silhouette Score.
- Compare clustering performance using evaluation metrics.
- Save the trained models and scalers.

## Dataset

The project uses the Wine dataset from the UCI Machine Learning Repository.

- **Total samples:** 178
- **Number of features:** 13
- **Learning type:** Unsupervised learning
- **Original classes:** 3

The features describe the chemical properties of wine, such as alcohol, malic acid, ash, magnesium, and color intensity.

The original `Class` column is used only to evaluate the clustering results, not to train the clustering models.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Joblib
- Jupyter Notebook

## Project Structure

```text
Wine_Clustering/
│
├── Data/
│   └── interim/
│       └── wine_cleaned.csv
│
├── models/
│   ├── kmeans_model.pkl
│   ├── kmeans_scaler.pkl
│   ├── hierarchical_model.pkl
│   └── hierarchical_scaler.pkl
│
├── notebooks/
│   └── model development/
│       ├── 02_kmeans_clustering.ipynb
│       ├── 03_hierarchical_clustering.ipynb
│       └── 04_clustering_model_comparison.ipynb
│
├── requirements.txt
└── README.md