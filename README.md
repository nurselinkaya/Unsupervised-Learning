# Clustering Analysis using KMeans Algorithm
## Introduction
This Python code performs a clustering analysis on a dataset using the KMeans algorithm. It imports the required libraries, reads in a CSV file containing the data, performs a simple data visualization, and then applies the KMeans algorithm to cluster the data into different groups. It is a very basic code, for the introduction of KMeans clustering for beginners.

## Libraries Used
The following libraries were imported for this code:

pandas for data manipulation and analysis
numpy for numerical operations
matplotlib.pyplot for data visualization
sklearn.cluster for applying the KMeans algorithm
scipy.spatial.distance for computing pairwise distances

## Dataset
The Ruspini data set, consists of 75 points in four groups, which is popular for illustrating clustering techniques. The dataset used in this code is located in the CSV file dataset-11814.csv. However, you can download the dataset also from the website:
https://r-data.pmagunia.com/dataset/r-dataset-package-cluster-ruspini

## Data Visualization
To viualize the datapoints and identify the outliers, scatterplot and boxplot methods from matplotlib.pyplot library have been used.

## Choosing the Optimal Number of Clusters
To choose the optimal number of clusters, elbow method has been used. The distortion (within-cluster sum of squares) for different values of n_clusters have been calculated and the results have been plotted. The user can then visually inspect the plot to determine the optimal number of clusters.

## Clustering Analysis
KMeans algorithm has been applied to cluster the data into different groups. After the KMeans object with the number of clusters to create (n_clusters) have been initialized, which was determined by the elbow method, and the model is fit to the data using the kmeans.fit() method, the cluster centers and the labels of the data points using the kmeans.cluster_centers_ and kmeans.labels_ attributes have been calculated.

After performing the clustering analysis, a scatter plot of the data points, colored according to their cluster label. and the cluster centers (centroids) on the same plot have been displayed.

## Conclusion
This code provides an example of how to perform a clustering analysis using the KMeans algorithm in Python. It also demonstrates how to visualize the data and choose the optimal number of clusters using the elbow method.
