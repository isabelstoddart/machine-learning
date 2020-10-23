# Machine Learning Assignment 1
## Classification, Natural Language
### Task: Predict toxic comments within the data set of Wikipedia comments

## Iteration 1
### Changes Made
* change n_features to (2**16) in HashingVectorizer
* change ngram_range to (1,2) in HashingVectorizer
* alternate_sign=False (doesn’t work with alternate_sign=True because NaiveBayes can’t take negative values)
* Add exclamation point count (toxic_data['exclaim_count'] = toxic_data["comment_text"].str.count(“\!”))
* Got rid of random forest classifier and ordinary least squares because they aren’t doing well
