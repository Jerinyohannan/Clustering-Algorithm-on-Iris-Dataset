# Clustering-Algorithm-on-Iris-Dataset
Clustering Algorithm on Iris Dataset using algorithms KMeans Clustering and Hierarchical Clustering

## Loading and Preprocessing 
Load the Iris dataset from Sklearn dataset
Preprocessing
Data is already cleaned, so no scaling is necessary for clustering.
Since this is clustering, we do not use the target column (species)
The Iris dataset has only 150 samples and 4 features

## Clustering Algorithm Implementation
### KMeans Clustering
KMeans is an unsupervised learning algorithm in machine learning where data points are grouped based on a predefined number of clusters called k. This aims to minimize the variance within the clusters by finding the k cluster centers, referred to as centroids, then assigning every data point to the nearest centroid. Minimize WCSS
Randomly initializes k centroids.
Assign each point to the nearest centroid.
Computing the centroids as the average of all points assigned to it.
Iterating until the centroids stabilize, or the maximum iterations are attained.

KMeans will have no difficulty in identifying this as the clusters are easy to pick up as it can handle simple low-dimensional datasets with clear separations between clusters.
The Iris dataset naturally splits into three clusters
corresponding to the three species of flowers.
KMeans works better for spherical and similarly sized clusters
which is the nature of the Iris dataset.

### Hierarchical Clustering
Hierarchical clustering is one of the unsupervised algorithms in which the machine learning algorithm forms a hierarchy of clusters either by merging smaller ones together or splitting larger ones. The representation of this is often in a dendrogram, showing the formation or splitting of clusters.Begin by creating a single cluster for each data point.Merge the closest clusters iteratively based on a distance metric.Continue till all points merge into one single cluster.

it is computationally feasible for hierarchical clustering. The benefit of hierarchical clustering is that it does not require giving the number of clusters in advance as does KMeans, making exploration convenient. The dendrogram explains the relationship of the data points and clusters,It does not require that one know beforehand the number of clusters (though we often cut the dendrogram at some level to decide upon our number of clusters).Dendrogram gives a visual representation of the hierarchical relationship among the points.
