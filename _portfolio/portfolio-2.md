---
title: "Patient Treatment Classfication"
excerpt: "Predicting Patient Outcomes using Electronic Health Record collected from a private Hospital in Indonesia - Classificatio Task (Kaggle)<br/><img src='/images/EHC_classification.jpg'>"
collection: portfolio
---

## Problem

Describe a persona [classify] of wether the next patient that is administered basic laboratory tests would require to be admitted in to the hospital (incare patient) or can be treated within the out-patient department of the hospital itself.

## Aims and Methods

For this classification my aim was to test a suite of supervisory classification algorithms, namely:

- Logistic Regression
- Support Vector Machine
- K-Nearest Neighbour
- Random Forest

  Used the 'SOURCE' column that classifies each patient as 'IN' or 'OUT' as the target variable for the classification process.

Following the classification with each of these methods, I evaluated each of these models using the following metrics:

- Accuracy: Provide the overall number of correct predictions divided by the total number of predictions.
- Confusion Matrix: A breakdown of predictions into a table showing correct predictions (the diagonal) and the types of incorrect predictions made (what classes incorrect predictions were assigned).
- Precision: A measure of a classifiers exactness.
- Recall: A measure of a classifiers completeness
- F2 Score (or F-score): A weighted average of precision and recall, with more importance to recall as we want to avoid false-negative errors more than false-positive errors.

## Results

In terms of accuracy i.e., the overall number of correct predictions, Random Forest shows a clear superiority with 76.8% followed by KNN with 74.9% and SVM with 74.7%.

Using the F2 score that bears more weight to the recall which shows the percentange of relevant data points correctly classified by the models, we again see Random Forest clearly win over KNN and SVM. Howevewr, SVM performs slightly better in predicting the out patient data (0.83) while KNN performs better in predicting the in patient data (0.64) between the two.

You can view the entire notebook of my work [here](https://www.kaggle.com/code/osbornepereira/ehc-classification).
