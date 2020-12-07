# Machine Learning Assignment 3
## Unsupervised, Clustering
### Task: Cluster Amazon food reviews to create a recommendation engine for Amazon products
## Iteration 1
### Changes Made
* Added strip_accents='ascii' to the CountVectorizer()
* Added stop_words='Enlgish' to the CountVectorizer()
* Added ngram_range=(1,2) to the CountVectorizer()
### Current Number of Clusters: 32
I am currently using 32 clusters. There are a lot of clusters on tea, coffee, chips etc., but the clusters are about different types of these products. As of now, I think more clusters is better to create more specific groups.
