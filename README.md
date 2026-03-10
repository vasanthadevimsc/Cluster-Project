# Cluster-Project
________________________________________
📊 Implementing and Comparing K-Means Clustering on Synthetic Data

# 📌 Project Overview

This project implements the K-Means clustering algorithm from scratch using NumPy and compares its performance with Scikit-learn’s optimized KMeans implementation.
A synthetic dataset is generated using sklearn.datasets.make_blobs with clearly separable clusters. The comparison is done using Silhouette Score and visual inspection of clusters and centroids.
________________________________________
# 🎯 Objectives

•	Generate a synthetic dataset with 4 distinct clusters

•	Implement K-Means clustering from scratch (NumPy only)

•	Apply Scikit-learn’s KMeans on the same dataset

•	Compare clustering quality using Silhouette Score

•	Visualize clusters and final centroids

•	Understand convergence behavior and initialization sensitivity
________________________________________
# 🧪 Dataset Description

The dataset is generated programmatically using make_blobs.

Parameter	Value

Number of samples	500

Number of clusters	4

Features	2

Standard deviation	1.2

Random state	42
________________________________________
# 🛠️ Technologies Used

•	Python 3.x

•	NumPy

•	Matplotlib

•	Scikit-learn
________________________________________
# 📂 Project Structure

kmeans-clustering-project/

│

├── kmeans_scratch.py        # K-Means implementation from scratch

├── main.py                  # Dataset generation, comparison & visualization

├── README.md                # Project documentation
________________________________________
# ⚙️ Implementation Details

🔹 Scratch K-Means (NumPy)

The custom K-Means implementation includes:

•	Random centroid initialization

•	Euclidean distance calculation

•	Cluster assignment

•	Centroid recalculation

•	Convergence check

•	Maximum iterations = 100

 Scikit-learn KMeans

•	Uses k-means++ initialization

•	Multiple initializations (n_init)

•	Optimized convergence
________________________________________
# 📈 Evaluation Metric

Silhouette Score is used to measure clustering quality.

•	Range: -1 to +1

•	Higher value → better cluster separation
________________________________________
# 📊 Results Summary

•	Scikit-learn KMeans generally achieves a slightly higher silhouette score

•	Scratch K-Means produces similar cluster shapes

•	Differences arise due to:

o	Initialization strategy

o	Optimization level

o	Multiple restarts in Scikit-learn
________________________________________
# 🖼️ Visualizations

The project includes:

•	Scatter plot of data points colored by cluster labels

•	Final centroids marked for:

o	Scratch K-Means

o	Scikit-learn KMeans

These plots help visually validate clustering quality.
________________________________________
# ▶️ How to Run

1.	Install dependencies:

2.	pip install numpy matplotlib scikit-learn

3.	Run the main script:

4.	python main.py
________________________________________
# 📚 Learning Outcomes

•	Deep understanding of the K-Means algorithm

•	Hands-on experience with NumPy-based implementation

•	Practical comparison with an industry-standard ML library

•	Insight into clustering evaluation metrics
________________________________________
# ✅ Conclusion

This project demonstrates that while a scratch implementation can effectively cluster data, Scikit-learn’s KMeans performs better due to optimized initialization and convergence techniques. Both approaches help build strong conceptual and practical understanding of unsupervised learning.
