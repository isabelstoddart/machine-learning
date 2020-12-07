# Machine Learning Assignment 3
## Unsupervised, Clustering
### Task: Cluster Amazon food reviews to create a recommendation engine for Amazon products
### Iteration 1
Changes Made
change image feature set representation from feature canny to HOG
change pixels_per_cell HOG parameter to (10,10)
change max_iter to 1000 where the multilayer perceptron is trained
add n_iter_no_change=100 where the multilayer perceptron is trained
add learning_rate='adaptive' where the multilayer perceptron is trained
add solver='lbfgs'
