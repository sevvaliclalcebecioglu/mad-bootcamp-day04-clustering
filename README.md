# 🚗 Day 04 - Car Clustering Project  
Project from the "Mastering Applied Data Science Bootcamp"  

This repository contains my study project on **clustering cars based on their similarities** using unsupervised learning techniques.  
The goal was to explore the dataset, apply multiple clustering algorithms, and identify meaningful groups of cars.

---

## 🔹 Project Overview
The project follows a structured workflow:

### Exploratory Data Analysis (EDA)
- Load and inspect car dataset (`cars.xls`)  
- Check dataset structure, sample rows, and missing values  
- Visualize distributions and relationships using scatter plots, countplots, and heatmaps  

### Feature Selection
- Selected features for clustering: `Price`, `Mileage`, `Cylinder`  
- Standardized features where necessary using `StandardScaler`  

---

## 🔹 Clustering Techniques Used
This project explores several unsupervised clustering techniques:

### 1. K-Means Clustering
- Partitions the dataset into `k` clusters by minimizing the variance within each cluster.  
- Suitable for spherical-shaped clusters and works well when the number of clusters is known.  
- Uses metrics like **WCSS (Within-Cluster Sum of Squares)** and **Silhouette Score** to evaluate clustering quality.  

### 2. Hierarchical Clustering
- Builds a hierarchy of clusters using either **agglomerative (bottom-up)** or **divisive (top-down)** methods.  
- Does not require pre-specifying the number of clusters.  
- Dendrograms are used to visualize cluster relationships and determine an optimal number of clusters.  

### 3. DBSCAN (Density-Based Spatial Clustering)
- Groups together points that are closely packed and marks points in low-density regions as outliers.  
- Effective for datasets with noise and clusters of arbitrary shapes.  
- Parameters include `eps` (distance threshold) and `min_samples` (minimum points to form a cluster).  

### 4. Agglomerative Clustering
- A type of hierarchical clustering that starts with each point as its own cluster and merges them iteratively.  
- Uses distance metrics like Euclidean distance and linkage methods like Ward’s method to minimize variance between clusters.  

### 5. Other Techniques
- **Mean Shift Clustering:** Identifies clusters by finding dense areas in the feature space.  
- **Gaussian Mixture Models (GMM):** Probabilistic model assuming data points are generated from a mixture of Gaussian distributions.  
- **Spectral Clustering:** Uses graph-based methods to identify clusters in non-convex datasets.  

---

## 🔹 Key Results
- Successfully grouped cars based on **Price, Mileage, and Cylinder**  
- Evaluated cluster quality using **Silhouette Score** and visual inspection  
- K-Means and Agglomerative Clustering produced clear, meaningful clusters  
- DBSCAN helped detect outliers and denser clusters  

---

## 🔹 Conclusion
This project demonstrates the power of **unsupervised learning** in identifying patterns in car datasets.  
By using multiple clustering algorithms, we can segment cars into meaningful groups for analysis, anomaly detection, or further business insights.
