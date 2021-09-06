# Tree-Based Classifiers
Application and performance evaluation for three tree-based classifiers: Decision Trees, Random Forests, and Gradient Tree Boosting, on two different datasets; 
Wheat Seeds and Covid-19 Outcomes in Ontario.


## Specific Objectives
- Load datasets and perform some exploratory plots.
- Application on the use of classification algorithms: decision tree, random forest,and XGBoost.
- Performance comparison and evaluation the three approaches


## Datasets
**Wheat Seeds:** This small dataset is the UCI Seeds Data set (https://archive.ics.uci.edu/ml/datasets/seeds). The examined group comprised kernels belonging to three different varieties of wheat: Kama, Rosa and Canadian. These are the labels. There are 70 elements for each variety of wheat, randomly selected for the experiment.

**Covid-19 Outcomes in Ontario:** Dataset 2 is about the confirmed COVID-19 cases in Ontario. A subset of this data is provided. The original data comes from the following file “Confirmed positive cases of COVID19 in Ontario” at: https://data.ontario.ca/dataset/confirmed-positive-cases-of-covid-19-in-ontario. This project
is using the features age group, gender, case acquisition info, city, outbreak, latitude, and longitude. The feature outcome1 is the label.


## Implementation
- Classify the data using three tree-based classifiers: Decision Trees, Random Forests and Gradient Tree Boosting.
- Tune the hyper-parameters of the classifier using 10-fold cross validation and sklearn functions.
- Evaluate the best value for the number of trees and maximum depth of trees.
- Across both datasets, compare and contrast the performance of the three approaches and highlight interesting patterns.

### Decision Trees:
- Max depth: {3, 5, 10, None}.
- Plot the mean accuracy versus the maximum depth. 
- Examine the final resulting splitting rules used for the trees and highlight interesting patterns that explain the data.

### Random Forest:
- Number of trees: {5, 10, 50, 150, 200}
- Max depth: {3, 5, 10, None}
- Plot the mean accuricies in a Heat Plot for different values of number of trees and maximum depth.

### Gradient Tree Boosting
- Use GradientBoostingClassifier on SKLearn
- Number of estimators: {5, 10, 50, 150, 200}
- plot the mean accuracy versus the number of estimators.
