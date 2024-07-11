# Cryptocurrency Market Clustering Analysis

This repository contains a Python script for performing clustering analysis on cryptocurrency market data. The analysis aims to identify groups of similar cryptocurrencies based on their market performance. The process includes data normalization, k-means clustering, and principal component analysis (PCA) for dimensionality reduction. The results are visualized using both the original features and the principal components.

## Prerequisites

Ensure you have the following libraries installed:

- pandas
- hvplot
- scikit-learn
- matplotlib

## Data

The dataset used in this analysis should be in the Resources directory with the filename crypto_market_data.csv. 

## Instructions:

1. Ensure that data file is located in correspoding folder or change the path to data file.

2. Import required libraries:
- import pandas as pd
- import hvplot.pandas
- from sklearn.cluster import KMeans
- from sklearn.decomposition import PCA
- from sklearn.preprocessing import StandardScaler
- import matplotlib.pyplot as plt

3. Run the script.

## Analysis Steps:

1. Normalize the data with `StandardScaler()`;
2. Determine the optimal number of clusters using the Elbow Method;
3. Fit the K-Means model and predict clusters using `KMeans`();
4. Visualize the clusters;
5. Reduce dimensionality using `PCA()`;
6. Determine the optimal number of clusters using PCA data with `KMeans`();
7. Fit the K-Means model using PCA data and predict clusters;
8. Visualize the PCA clusters;
9. Create composite Elbow Curve plot and Cluster plot to compare methods.

## Results
The script identifies clusters of cryptocurrencies based on their market performance. It uses the Elbow Method to determine the optimal number of clusters.Both the original data and PCA-reduced data are used for clustering, allowing comparison of the clustering results. The clusters are visualized using scatter plots to help identify patterns and similarities among the cryptocurrencies.
