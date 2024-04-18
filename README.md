# Classification of Patient with Depressive Disorder
## Project Overview

## Data
The dataset we are using is sourced from a 2020 Behavioral Risk Factor Surveillance System (BRFSS) Survey Data, and modified before being provided. The dataset initially had 5000 tuples with 276 attributes in total.

## Training Datasets

We used 2 different data balancing techniques and 3 different attribute selection methods. We created the training sets for each combination of those balancing methods
and attribute selection methods, thus there are 6 training sets prepared in total.

The combination of methods are as follows:

Training Set 1: SMOTE and CFS
Training Set 2: SMOTE and info gain
Training Set 3: SMOTE and RF importance
Training Set 4: Random over/under sampling and CFS
Training Set 5: Random over/under sampling and info gain
Training Set 6: Random over/under sampling and RF importance

## Classification Models

Using 6 different training datasets prepared above, we used 6 diffferent classification models below to fit the each of dataset. Thus, we created 36 models in total.

1. Recursive Partitioning Classification
2. Logistic Regression
3. Naive Bayes
4. Random Forest
5. Linear Discriminany Analysis
6. Support Vector Machine 

## Evaluation/Result

We have fitted 36 different models in total, and found the performance measures for each model. In choosing the best model, we first shortlisted the models having 0.6 or above class Y TPR and 0.7 or above class N TPR. We found that all of the shortlisted models performed similarly well in terms
of Precision, Recall, F-Measure, and ROC. However, when we consider Matthews Correlation Coefficient (MCC) and Kappa, Model 5 of Logistic Regression stands out slightly with higher values, suggesting better overall accuracy and agreement.


## Source Code
The code is in R (https://github.com/ssunami/classification-depressive-disorder/blob/main/Depressive_Disorder_Project.Rmd). This can be downloaded locally though requires installing R and R Studio.

## Project Report
Full project report is available here (https://github.com/ssunami/classification-depressive-disorder/blob/main/Depressive_Disorder_Project.pdf)



