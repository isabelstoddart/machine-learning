# Machine Learning Assignment 2
## Classification, Images
### Task: Train a model to best predict the presence of an aircraft in an image

## Iteration 1
### Changes Made
* change image feature set representation from feature canny to HOG
* change pixels_per_cell HOG parameter to (10,10)
* change max_iter to 1000 where the multilayer perceptron is trained
* add n_iter_no_change=100 where the multilayer perceptron is trained
* add learning_rate='adaptive' where the multilayer perceptron is trained
* add solver='lbfgs'
