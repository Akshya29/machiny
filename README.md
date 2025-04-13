# Gene Expression-Based Classification and Clustering Using Machine Learning
This page demonstrates the basics of how a machine learning model (Random Forest) can be used to classify gene expression data and cluster similar genes together using UMAP.

# Random Forest
A Random Forest is a machine learning method that builds multiple decision trees, each trained on a different random subset of the data. Predictions are made by combining the results of all the trees, which improves accuracy and stability. Each tree chooses the best place to split the data using a metric like Gini impurity.
Gini impurity measures how "impure" a node is in a decision tree using the formula:

Gini=1−∑( P<sub>i</sub><sup>2</sup>)

# UMAP (Uniform Manifold Approximation and Projection) 
Dimension reduction is a major tool for machine learning models to visualize and understand high-dimensional datasets. UMAP is one such widely used technique. It constructs a graph representation of the data, preserving the local structure by connecting nearby points. UMAP then reduces the dimensionality by projecting these points into a lower-dimensional space, typically 2D or 3D, while maintaining both the local and global relationships between data points, allowing for better interpretation and visualization.

# K-Means Clustering
K-means clustering is an unsupervised learning method used to group data points into K clusters. Initially, K centroids are randomly chosen, each representing a cluster. Then, each data point is assigned to the nearest centroid based on distance (usually Euclidean distance). After this, the centroid of each cluster is recalculated as the mean of all the data points within that cluster. This process of assigning points to clusters and updating centroids is repeated iteratively until the clusters stabilize, meaning the data points no longer change clusters.

# data used 
The data used here is from Scott et al., 2016 (Supplemental Information Supplemental File 1: tpg2plantgenome2015040025-sup-0001.xlsx). This data included gene expression data across various zones of maize roots as well as the clusters these genes belongs to. Hence used as an input to train a model to predict the genes in different nodes using Random Forest and Group the similar Clusters using K-Means Clustering.

# References
Stelpflug, S. C., Sekhon, R. S., Vaillancourt, B., Hirsch, C. N., Buell, C. R., de Leon, N., & Kaeppler, S. M. (2016). An Expanded Maize Gene Expression Atlas based on RNA Sequencing and its Use to Explore Root Development. The plant genome, 9(1), 10.3835/plantgenome2015.04.0025. https://doi.org/10.3835/plantgenome2015.04.0025
Pedregosa, F., Varoquaux, G., Gramfort, A., Michel, V., Thirion, B., Grisel, O., ... & Duchesnay, É. (2011). Scikit-learn: Machine learning in Python. *Journal of Machine Learning Research*, *12*, 2825-2830. http://www.jmlr.org/papers/volume12/pedregosa11a/pedregosa11a.pdf
W3Schools. (n.d.). Python Machine Learning - K-Means. W3Schools. Retrieved April 13, 2025, from https://www.w3schools.com/python/python_ml_k-means.asp
McInnes, L., & Healy, J. (2020). Understanding UMAP. PAIR. Retrieved April 13, 2025, from https://pair-code.github.io/understanding-umap/

