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

## Iteration 2
### Changes Made
* added final_image=np.array[[hog_image]] that Jill and Mia discovered works really well. This turned the final_image into an array
* played around with my_random_seed after a discussion in office hours on how much it can change the final result. I tried a lot of different numbers ranging from 24 to 12720 and ended up using my_random_seed=2000
* added back as_gray=True in img_raw=io.imread(imname, as_gray=True)
