

Clustering is the task of grouping similar data points together based on particular traits. 


# Types of clustering algorithms

**Connectivity models:** Data points closer in data space are more similar that data points lying farther away. Two methods:

- Classify each data point as a separate cluster, then aggregate one by one based on closest distance
- Put all data points in a single cluster, then partition based on farthest distance

**Centroid Models (K-Means Clustering):** Iterative clustering algorithms; similarity is derived by closeness of data to centroid of clusters.


**Distribution Models (EM algorithm):** Cluster based on probability of membership to the same distribution

**Density Models (DBScan):** Search data space for areas of varied density of data points in the data space

# Algorithms overview

## K-Means Clustering

Suitable for bigger datasets. High variance algorithm, due to randomization of clusters. Need to define hyperparameter K. 

1. Specify number of desired clusters K
2. Randomly assign each data point to a cluster
3. Compute centroids
4. Assign each point to closest cluster centroid
5. Repeat steps 3, 4 until no points change

## Hierarchical Clustering

Hierarchical clustering builds a hierarchy of clusters by merging (agglomerative) or splitting them successively (divisive). Suitable for smaller datasets, and data that has a non-flat structure.

### Agglomerative

1. Assign each data point to its own cluster
2. Merge nearest clusters
3. Repeat 2 until there is only one cluster left


### Divisive

1. Assign all data points to one cluster
2. Parition cluster into two based on distance
3. Repeat step 2 for every sub cluster, until each point is in its own cluster






# Appendix

**Hard and soft clustering:** In hard clustering, data points are assigned absolutely to a particular grouping. In soft clustering, each data point is assigned a probability of being assigned to a group. 