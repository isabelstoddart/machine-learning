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
