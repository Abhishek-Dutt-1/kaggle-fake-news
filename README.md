# Kaggle Fake News Classification:

**## Solution Notebook:**
GitHub preview: [fake_news_classifier.ipynb](https://github.com/AbhishekDutt/kaggle-fake-news/blob/master/fake_news_classifier.ipynb)

Google Colab: [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AbhishekDutt/kaggle-fake-news/blob/master/fake_news_classifier.ipynb)


## Solution Details:

**SVM** classifier with **TF-IDF** word vectors was the best performing model.

Other word vectors and classifiers tried were: 

**Word vectors:**
1. Count Vectors
2. TF-IDF
3. Word2Vec
4. GloVe

**Classification methods:**
1. Logistic Regression
2. KNN
3. SVM
4. RandomForest
5. XGBoost
6. LSTM 

Model with the highest accuracy on the unseen validation set was selected. <br/>
Model hyperparameters were tuned using Grid Search with Cross Validation.


## Evaluation Metrics:

Final model had following metrics on validation set:

**AUC ROC:** 97%

**Confusion Matrix:**

|  |  |Actual|Actual|
|:-:|:-:|:-:|:-:|
|  |  |1  |  0|
|Pred|1 |1,995|65|
|Pred|0 |41|2,059|

**Precision-Recall:**

|Label | Precision | Recall|
|:-:|:-:|:-:|
|0 | 0.97 | 0.98|
|1 | 0.98 | 0.97|

