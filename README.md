# Beyond Analysis

## EDA/FEATURE ENGINEERING
1. We are using pandas profiling library to generate reports on our training dataset. [Source](https://pypi.org/project/pandas-profiling/)
2. On analysis we found out columns of the dataset to be positively skewed , hence we decided to normalize the dataset using Power and Logarithmic transformation
3. We decided to group the data on the basis of "unique identifier" column to improve the variance of the "Y1" and "Y2" metrics.
4. We have used label encodings on the categorical feature columns.

## MODELS AND NOTEBOOKS
1. We decided to use three models catboost,lightbgm and xgboost and we took the arithmetic mean of their respective predicted values and used them as the final submission.
   - [Ensembling of Models](https://www.kaggle.com/gaurangthakur/beyond-analysis-1)

2. We decided to hypertune the model by using optuna hypertuning but it didn't gave the desired results.

3. We finally used sequential model (neural network) where we used :
   - Two hidden layers with activation ="relu" 
   - Optimizer = "adam"
   - [Neural Network Notebook](https://www.kaggle.com/gaurangthakur/beyond-analysis-2)
  
## Scope for Improvement:
1. Better Feature engineering can be done.
2. We could have used better deeplearning models such as lstm ,rnn etc..
 
