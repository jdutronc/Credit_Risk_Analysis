# Credit_Risk_Analysis

## Project Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we will need to employ different techniques to train and evaluate models with unbalanced classes. In this challenge, we use python to build several machine learning models, then evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk:

1. oversample the data using the RandomOverSampler and SMOTE algorithms;
2. undersample the data using the ClusterCentroids algorithm;
3. use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm;
4. compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.


## Results

### Oversample the data with RandomOverSampler

<table align="left">
  <tr height=50px>
    <th>Accuracy Score</th>
    <th>Confusion Matrix</th>
    <th>Classification Report</th>
  </tr>
  <tr>
    <td> <img src='Resources/Oversampling_AccScore.png'>
    <td> <img src='Resources/Oversampling_ConfMatrix.png'>
    <td> <img src='Resources/Oversampling_ClassReport.png'>
  </tr>
</table>
<br> 
  
- balanced accuracy score is 64%.
- high_risk precision is about 1% only with 60% sensitivity
- F1 is very low at 2% only.
<br clear="left"/>

### Oversample the data with the SMOTE algorithm

<table align="left">
  <tr height=50px>
    <th>Accuracy Score</th>
    <th>Confusion Matrix</th>
    <th>Classification Report</th>
  </tr>
  <tr>
    <td> <img src='Resources/SMOTE_AccScore.png'>
    <td> <img src='Resources/SMOTE_ConfMatrix.png'>
    <td> <img src='Resources/SMOTE_ClassReport.png'>
  </tr>
</table>
<br> 

- balanced accuracy score is 64%.
- high_risk precision is about 1% only with 60% sensitivity
- F1 is very low at 2% only.
<br clear="left"/>

### Undersample the data with the ClusterCentroids algorithm

<table align="left">
  <tr height=50px>
    <th>Accuracy Score</th>
    <th>Confusion Matrix</th>
    <th>Classification Report</th>
  </tr>
  <tr>
    <td> <img src='Resources/Undersampling_AccScore.png'>
    <td> <img src='Resources/Undersampling_ConfMatrix.png'>
    <td> <img src='Resources/Undersampling_ClassReport.png'>
  </tr>
</table>
<br> 

- balanced accuracy score is 64%.
- high_risk precision is about 1% only with 60% sensitivity
- F1 is very low at 1% only.
<br clear="left"/>

### Over- and undersampling with the SMOTEENN algorithm

<table align="left">
  <tr height=50px>
    <th>Accuracy Score</th>
    <th>Confusion Matrix</th>
    <th>Classification Report</th>
  </tr>
  <tr>
    <td> <img src='Resources/SMOTEENN_AccScore.png'>
    <td> <img src='Resources/SMOTEENN_ConfMatrix.png'>
    <td> <img src='Resources/SMOTEENN_ClassReport.png'>
  </tr>
</table>
<br> 

- balanced accuracy score is 52%.
- high_risk precision is about 1% only with 70% sensitivity
- F1 is very low at 2% only.
<br clear="left"/>

### BalancedRandomForestClassifier

<table align="left">
  <tr height=50px>
    <th>Accuracy Score</th>
    <th>Confusion Matrix</th>
    <th>Classification Report</th>
  </tr>
  <tr>
    <td> <img src='Resources/BRFC_AccScore.png'>
    <td> <img src='Resources/BRFC_ConfMatrix.png'>
    <td> <img src='Resources/BRFC_ClassReport.png'>
  </tr>
</table>
<br> 

- balanced accuracy score is 79%.
- high_risk precision is about 4% only with 67% sensitivity
- F1 is higher at 7%
<br clear="left"/>

### EasyEnsembleClassifier

<table align="left">
  <tr height=50px>
    <th>Accuracy Score</th>
    <th>Confusion Matrix</th>
    <th>Classification Report</th>
  </tr>
  <tr>
    <td> <img src='Resources/EEC_AccScore.png'>
    <td> <img src='Resources/EEC_ConfMatrix.png'>
    <td> <img src='Resources/EEC_ClassReport.png'>
  </tr>
</table>
<br> 

- balanced accuracy score is 93%.
- high_risk precision is about 7% only with 91% sensitivity
- F1 is much higher at 14%
<br clear="left"/>

## Summary

