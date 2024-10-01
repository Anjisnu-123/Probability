<!--Hierarchical clustering: concept of hierarchical lustering,similarity distance measure,Linkage methods: single linkage,complete linkage,average linkage,Ward's method,building the 
dedogram,Steps to build a dedogram(1. Start with inidividual data point 2.Merge the closest clusters 3. Repeat untilll alll points are in a single clusters,cut the dedogram in a appropiate level),Hierchical clustering example,Explanation,cutting the dedogram from cluster.

Hierchichal clustering for multivare data in EDA: Uncovering natural grouping,visualizing multivariate relationships with dedogram,dimensionality and hierarchical clustering:PCA,factor analysis,Exploring varriable in relationship

t-SNE: overview,Math behind t-sne: HIgh dimensional space,low dimensional space,cost function: it minimizes the kullback leibar divergence between the two distributions,optimization,Application in EDA

k-means clustering: overview,Math behind k means: intialization,Assignment step,update step,iterate,application in EDA

Multidimensional scaling(MDS):overview,math behind MDS:distance matrix,config in low dimensional space,objective function,optimization,Appplication in EDA.

Factor analysis: overview,math behind factor analysis: model representation,covariance matrix,estimation, Application in EDA

canonical correlation analysis: overview,math behind CCA,linear combination,objective function,Eigen value problem, Application in EDA


Day 15: Hypothesis testing and parameter estimation -->

# Clustering and Dimensionality Reduction Techniques in EDA

## Hierarchical Clustering

### Concept of Hierarchical Clustering
Hierarchical clustering is a method of cluster analysis that seeks to build a hierarchy of clusters. It is typically represented as a dendrogram, which illustrates the arrangement of the clusters.

### Similarity Distance Measure
Common measures of similarity (or distance) include:
- **Euclidean Distance**: The straight-line distance between two points in Euclidean space.
- **Manhattan Distance**: The sum of the absolute differences of the coordinates.
- **Cosine Similarity**: Measures the cosine of the angle between two vectors.

### Linkage Methods
1. **Single Linkage**: Measures the distance between the closest points in two clusters.
2. **Complete Linkage**: Measures the distance between the farthest points in two clusters.
3. **Average Linkage**: Uses the average distance between all pairs of points in two clusters.
4. **Ward's Method**: Minimizes the total within-cluster variance.

### Building the Dendrogram
A dendrogram is constructed by the following steps:
1. **Start with Individual Data Points**: Each data point is its own cluster.
2. **Merge the Closest Clusters**: Based on the chosen linkage method.
3. **Repeat Until All Points are in a Single Cluster**: Continue merging until only one cluster remains.
4. **Cut the Dendrogram at an Appropriate Level**: Determine the desired number of clusters.

### Hierarchical Clustering Example
- **Explanation**: A dataset of species can be clustered to show similarities in their characteristics.
- **Cutting the Dendrogram**: Determine clusters by cutting the dendrogram at a specific height.

---

## Hierarchical Clustering for Multivariate Data in EDA

### Uncovering Natural Grouping
Hierarchical clustering helps identify natural groupings in multivariate datasets.

### Visualizing Multivariate Relationships with Dendrograms
Dendrograms allow visualization of how clusters are formed based on similarities.

### Dimensionality and Hierarchical Clustering
- **PCA (Principal Component Analysis)**: Reduces the dimensionality of the data before clustering.
- **Factor Analysis**: Identifies underlying relationships between variables.
- **Exploring Variable Relationships**: Analyzing how variables interact within clusters.

---

## t-SNE (t-Distributed Stochastic Neighbor Embedding)

### Overview
t-SNE is a nonlinear dimensionality reduction technique primarily used for visualizing high-dimensional data.

### Math Behind t-SNE
- **High-Dimensional Space**: Represents the original data points.
- **Low-Dimensional Space**: Represents the embedding of data points.
- **Cost Function**: Minimizes the Kullback-Leibler divergence between the probability distributions of the high-dimensional and low-dimensional representations.
- **Optimization**: Utilizes gradient descent to minimize the cost function.

### Application in EDA
t-SNE is particularly useful for visualizing clusters in high-dimensional data, making patterns and groupings more apparent.

---

## K-Means Clustering

### Overview
K-means is a partitioning method that divides a dataset into K clusters based on feature similarity.

### Math Behind K-Means
1. **Initialization**: Choose K initial centroids randomly.
2. **Assignment Step**: Assign each data point to the nearest centroid.
3. **Update Step**: Recalculate centroids as the mean of assigned points.
4. **Iterate**: Repeat assignment and update steps until convergence.

### Application in EDA
K-means is used to find patterns and group similar observations in the data.

---

## Multidimensional Scaling (MDS)

### Overview
MDS is a technique used to visualize the level of similarity of individual cases of a dataset.

### Math Behind MDS
- **Distance Matrix**: A matrix of pairwise distances between points.
- **Configuration in Low-Dimensional Space**: Positions points in a lower-dimensional space to preserve distances.
- **Objective Function**: Minimizes the stress function, representing discrepancies between distances.
- **Optimization**: Achieved using iterative algorithms.

### Application in EDA
MDS is effective for visualizing complex datasets and understanding relationships among items.

---

## Factor Analysis

### Overview
Factor analysis is used to identify underlying relationships between variables.

### Math Behind Factor Analysis
- **Model Representation**: Data is represented as linear combinations of factors.
- **Covariance Matrix**: Analyzes the variance shared among variables.
- **Estimation**: Factors are estimated based on observed data.

### Application in EDA
Used to reduce the dimensionality of data and identify latent variables influencing observed measurements.

---

## Canonical Correlation Analysis (CCA)

### Overview
CCA is a method used to explore the relationships between two multivariate sets of variables.

### Math Behind CCA
- **Linear Combination**: Seeks linear combinations of two sets of variables that are maximally correlated.
- **Objective Function**: Maximizes the correlation between the linear combinations.
- **Eigenvalue Problem**: Solving the eigenvalue problem helps identify the optimal linear combinations.

### Application in EDA
CCA is useful for examining the relationships between two sets of variables and understanding their interactions.

---

## Conclusion

These clustering and dimensionality reduction techniques provide powerful tools for exploratory data analysis, helping to uncover patterns and relationships within complex datasets. By understanding the underlying mathematics, analysts can apply these methods effectively to derive insights from their data.
