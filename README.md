# CustomersClustering

**Context**

This dataset groups the customers of a bank. The objective is to find clusters of similar clients and identify certain main type of customers.

**Solution**

The solution utilizes the KMedoids algorithm with the Gower distance as metric due to the presence of relevant categorical features. The number of clusters is selected through the silhouette score, which is the chosen performance metric. Randomized Search Cross Validation is used to find sub-optimal parameters (Gower distance weights and number of clusters).

**Results**

The algorithm propose 9 cluster with an average silhouette score on the test set of 0.88. From a business perspective we can unite some of these clusters since the differences between them aren't related to the business aim. The final proposed business solution is composed by 6 different clusters.
