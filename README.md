# Gene Expression Analysis with PCA and KMeans Clustering

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Principal Component Analysis (PCA)](#principal-component-analysis-pca)
    1. [Variance Explained](#variance-explained)
    2. [PCA Components Plot](#pca-components-plot)
4. [KMeans Clustering](#kmeans-clustering)
    1. [KMeans on Original Features](#kmeans-on-original-features)
    2. [KMeans on PCA Components](#kmeans-on-pca-components)
5. [Comparison and Evaluation](#comparison-and-evaluation)
6. [Conclusion](#conclusion)

## Introduction
This project involves the application of Principal Component Analysis (PCA) and KMeans clustering on the **Gene Expression Cancer RNA-Seq Dataset** from UCI Machine Learning Repository. PCA is used to reduce the dimensionality of the gene data, while KMeans clustering is applied to both the original features and the PCA-reduced data to compare clustering performance.

## Dataset
The dataset used in this analysis is the [Gene Expression Cancer RNA-Seq Dataset](https://archive.ics.uci.edu/dataset/401/gene+expression+cancer+rna+seq), which contains RNA-Seq data for various types of cancer. The dataset consists of gene expression data, where rows correspond to samples, and columns correspond to different gene expression levels.

- **Source**: UCI Machine Learning Repository
- **Link**: [Gene Expression Cancer RNA-Seq Dataset](https://archive.ics.uci.edu/dataset/401/gene+expression+cancer+rna+seq)
- **Description**: This dataset contains RNA-Seq gene expression levels of patients from different cancer types.

## Principal Component Analysis (PCA)
PCA is applied to reduce the high-dimensional gene expression data into three principal components, capturing most of the variance in the dataset.

### PCA Components Plot
The first three principal components are plotted to visualize the reduced dataset in 3D space.

## KMeans Clustering
KMeans clustering is applied to both the original gene expression data and the PCA-reduced data to compare clustering performance using metrics like ARI (Adjusted Rand Index) and NMI (Normalized Mutual Information).

### KMeans on Original Features
ARI for KMeans on original features: 0.63  
NMI for KMeans on original features: 0.76

### KMeans on PCA Components
ARI for KMeans on PCA-transformed data: 0.55  
NMI for KMeans on PCA-transformed data: 0.69

## Comparison and Evaluation
- KMeans clustering on the original features performed slightly better, with higher ARI and NMI scores.
- PCA-reduced data still performed well, providing a balance between dimensionality reduction and clustering accuracy.

## Conclusion
PCA is effective in reducing the dimensionality of gene expression data while retaining most of the relevant information. KMeans clustering on both the original and PCA-reduced data shows good performance, with the original features providing more detailed clustering but at the cost of computational complexity.
