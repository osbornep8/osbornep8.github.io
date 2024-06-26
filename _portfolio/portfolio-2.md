---
title: "Patient Treatment Classification"
excerpt: "Predicting Patient Outcomes using Electronic Health Record collected from a private Hospital in Indonesia - Classification Task (Kaggle)<br/><img src='/images/EHC_classification.jpg'>"
collection: portfolio
---

## Overview

Tasked with predicting whether patients, based on initial lab tests, require hospital admission or outpatient care.

## Strategy and Execution

Tested a battery of advanced machine learning classifiers to address this challenge:

- **Logistic Regression**
- **Support Vector Machine**
- **K-Nearest Neighbour**
- **Random Forest**

Targeted the 'SOURCE' attribute to distinguish 'IN' (admitted) from 'OUT' (outpatient) cases.

Following the classification with each of these methods, I evaluated each of these models using the following metrics:

- **Accuracy**: Provide the overall number of correct predictions divided by the total number of predictions.
- **Confusion Matrix**: A breakdown of predictions into a table showing correct predictions (the diagonal) and the types of incorrect predictions made (what classes incorrect predictions were assigned).
- **Precision**: A measure of a classifier's exactness.
- **Recall**: A measure of a classifier's completeness
- **F2 Score (or F-score)**: A weighted average of precision and recall, with more importance to recall as we want to avoid false-negative errors more than false-positive errors.

## Results

In terms of accuracy i.e., the overall number of correct predictions, Random Forest shows a clear superiority with **76.8%** followed by KNN with **74.9%** and SVM with **74.7%**.

Using the F2 score that bears more weight to the recall which shows the percentage of relevant data points correctly classified by the models, we again see the Random Forest model clearly win over the KNN and SVM models. However, SVM performs slightly better in predicting the out-patient data (0.83) while KNN performs better in predicting the in-patient data (0.64) between the two.

You can view the entire notebook [here](https://www.kaggle.com/code/osbornepereira/ehc-classification).
