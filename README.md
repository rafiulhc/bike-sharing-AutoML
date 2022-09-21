# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Rafiul Hasan Chowdhury

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
Changing in time limits, evaluation metrics, presets come with different results. If any of my predictor have negative value, I've to change them into zero as Kaggle don't accept negative values as submission.

### What was the top ranked model that performed?
WeightedEnsemble_L3

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
Exploratory data analysis helps visulize and analyse data for better understanding.

### How much better did your model preform after adding additional features and why do you think that is?
Moderately and that was for changed in hyperparameters.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
0.20

### If you were given more time with this dataset, where do you think you would spend more time?
In the time limit parameter.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|600|"best_quality"|"False|1.7749|
|add_features|600|"best_quality"|"False|1.8001|
|hpo|600|"high_quality"|"True"|2.0201|

### Create a line plot showing the top model score for the three (or more) training runs during the project.



![model_train_score](https://user-images.githubusercontent.com/68476971/191481945-3d4910ea-f532-43b1-a084-b98f0f318485.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.


![model_test_score](https://user-images.githubusercontent.com/68476971/191440524-1c580a60-82df-416f-a99b-e80908134e58.png)

## Summary

AutoGluon is a beginer frienfly AutoML tool that uses  to train extremely accurate machine learning models on unprocessed tabular datasets like CSV files. AutoGluon succeeds by assembling several models and stacking them in various layers, unlike other AutoML frameworks that largely focus on model/hyperparameter selection. With hyperparameter tuning we can find better score.
