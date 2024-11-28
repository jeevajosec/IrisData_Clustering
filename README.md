# Hierarchical Clustering on Iris Dataset
Overview
This repository contains the code for performing Hierarchical Clustering on the famous Iris dataset using Python. Hierarchical Clustering is an unsupervised machine learning technique used to group similar data points based on their features. The goal of this project is to explore the effectiveness of Hierarchical Clustering on the Iris dataset and to visualize the clusters.

Dataset
Iris Dataset from sklearn library.
Features include sepal length, sepal width, petal length, and petal width of Iris flowers.
The target column "species" is removed, as this is a clustering problem.

Load and Preprocess Data:

Load the Iris dataset from sklearn.
Drop the "species" column since this is a clustering task.

Hierarchical Clustering Algorithm Implementation:
Perform Hierarchical Clustering using the Ward method to minimize variance within clusters.
Determine the optimal number of clusters using the silhouette score.

Evaluation:
Evaluate the quality of clusters using metrics like Silhouette Score, Calinski-Harabasz Index, and Davies-Bouldin Index.
Visualize the results using scatter plots or dimensionality reduction techniques (PCA, t-SNE).

Visualization:
Visualize clusters using scatter plots for 2D data, or PCA/t-SNE for high-dimensional data.
Optionally, visualize the dendrogram to see the hierarchical structure.

Workflow
Load the Data: Use the Iris dataset from sklearn and preprocess it by removing the "species" column.

Hierarchical Clustering:
Generate a linkage matrix using the linkage() function from scipy.cluster.hierarchy.
Assign cluster labels based on a specified number of clusters using the fcluster() function.

Evaluate Clustering Quality:
Compute silhouette scores and visualize cluster quality metrics.

Visualize Clusters:
Plot clusters in a 2D space with scatter plots or apply dimensionality reduction techniques (PCA, t-SNE).

Determine Optimal Number of Clusters:
Find the highest silhouette score, cut the dendrogram at the appropriate level, and visualize clusters.

Results
The silhouette score for Hierarchical Clustering provides a measure of how well-defined the clusters are.
Optimal number of clusters can be determined by examining the silhouette score plots and comparing different numbers of clusters.

Results Visualization
Silhouette Scores Plot: Displays the variation in silhouette scores for different cluster numbers.

Scatter Plot: Shows the data points colored by their assigned cluster label.

Dendrogram: Visualizes the hierarchical clustering tree to help determine the number of clusters.
