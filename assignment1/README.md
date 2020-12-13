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

## Final Iteration

My final iteration uses the ridge regression classifier with stochastic gradient descent and alpha value of 10. My hashing vectorizer parameters include n_features=(2xx6), alternate_sign=True, and ngram_range=(1,2). I am using additional features exclaim_count and s_count to count the number of exclamation points and the number of times the word shit occurs. I went through a few different models before ending with ridge regression. Some runner ups were the perceptron model, svm, and logistic regression. The ridge regression classifier ended up doing the best. It has a very high true positive rate, which sacrifices the false positive rate but I think that is okay, especially here where it is more important to tag a comment as toxic even if it is not actually toxic. It is better to be safe than sorry.
