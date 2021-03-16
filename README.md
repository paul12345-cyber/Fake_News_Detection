## Using Natural Language Processing (NLP) for Fake News Detection

We have applied machine learning to detect fake news on dataset obtained from [kaggle](https://www.kaggle.com/c/fake-news/data).
After cleaning and performing NLP functions on the data, we tested three classification models for optimal parameters using
Pipeline and Gridsearch. Highest accuracy score for the optimal model was 93.3%

## Methodology
* Data acquasition from Kaggle
* Data exploration. E.g, Finding most active authors
* Natural language processing
  * Stemming
  * Removing stopwords
  * removing non-alphanumeric characters
  * Count vectorize data
* Modeling: with pipeline and Gridsearch

## Model Performance:

 
#### Model 1: Best accuracy and score
- Support Vector Machince
- Best parameters are : {'C': 9, 'kernel': 'rbf'}
- Train score: 0.934
- Test score: 0.933


#### Model 2: 
- Random Forest
- Best parameters are : {'criterion': 'gini', 'max_depth': 10, 'min_samples_split': 10}
- Train score: 0.888
- Test score: 0.897


#### Model 3: 
- Logistic Regression
- Best params are : {'C': 1.0, 'penalty': 'l1', 'solver': 'liblinear'}
- Train score: 0.923
- Test score: 0.924
