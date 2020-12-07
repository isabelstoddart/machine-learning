# Machine Learning Assignment 1
## Classification, Natural Language
### Task: Predict toxic comments within the data set of Wikipedia comments

## Iteration 1
### Changes Made
* change n_features to (2**16) in HashingVectorizer
* change ngram_range to (1,2) in HashingVectorizer
* change alternate_sign to True in HashingVectorizer
* Add exclamation point count (toxic_data['exclaim_count'] = toxic_data["comment_text"].str.count(“\!”))
* Add count for the word "shit" (toxic_data["s_count"] = toxic_data["comment_text"].str.count("shit") + toxic_data["comment_text"].str.count("SHIT"))
* Working with perceptron as my model as of now
* get rid of word count
* get rid of punctuation count

## Iteration 2
### Changes Made
* change model from Perceptron to SVM LinearSVC
* change C to C=1000

## Iteration 3
### Changes Made
* tried to make an ensemble model with SVM, Perceptron, Ridge Regression, and Logistic Regression to see what the results would be. After making this ensemble, while playing around with these four models to get them all to perform better I realized ridge regression performs better than them all with some changes, primarily when using Stochastic Gradient descent
* Added solver='sag' (Stochastic Gradient descent) to ridge regression
* Added normalize=True to ridge regression because normalizing helps when using Stochastic Gradient descent
* Played around with alpha values and found that alpha=10 had the best true positive rate, so I set alpha=10
