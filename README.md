# Credit_Risk_Analysis

## Overview

The purpose of this analysis was to use machine learning methods on a dataset to see if we could create a model that predicts the credit risk of a certain person based on other metrics such as loan amount or income.  We used multiple sampling techniques to create different models in order to see what the best option was to predict the credit risk.

## Results

### Random Oversampling

<img src="https://github.com/bwheeler98/Credit_Risk_Analysis/blob/c686daf450aa58a8c1942785f26c8c2ae7f64d50/Screen%20Shot%202022-07-17%20at%203.28.11%20PM.png" width="500" height="350">

- Balanced Accuracy Score: 0.50
- High Risk Precision Score: 0.50
- Low Risk Precision Score: 0.99
- High Risk Recall Score: 0.01
- Low Risk Recall Score:  1.00

### SMOTE

<img src="https://github.com/bwheeler98/Credit_Risk_Analysis/blob/c686daf450aa58a8c1942785f26c8c2ae7f64d50/Screen%20Shot%202022-07-17%20at%203.28.34%20PM.png" width="500" height="350">

- Balanced Accuracy Score: 0.65
- High Risk Precision Score: 0.01
- Low Risk Precision Score: 1.00
- High Risk Recall Score: 0.61
- Low Risk Recall Score: 0.69

### Undersampling

<img src="https://github.com/bwheeler98/Credit_Risk_Analysis/blob/c686daf450aa58a8c1942785f26c8c2ae7f64d50/Screen%20Shot%202022-07-17%20at%203.28.47%20PM.png" width="500" height="350">

- Balanced Accuracy Score: 0.65
- High Risk Precision Score: 0.01
- Low Risk Precision Score: 1.00
- High Risk Recall Score: 0.69
- Low Risk Recall Score: 0.40

### SMOTEENN

<img src="https://github.com/bwheeler98/Credit_Risk_Analysis/blob/c686daf450aa58a8c1942785f26c8c2ae7f64d50/Screen%20Shot%202022-07-17%20at%203.28.57%20PM.png" width="500" height="350">

- Balanced Accuracy Score: 0.66
- High Risk Precision Score: 0.01
- Low Risk Precision Score: 1.00
- High Risk Recall Score: 0.75
- Low Risk Recall Score: 0.56

### Balanced Random Forest Classifier

<img src="https://github.com/bwheeler98/Credit_Risk_Analysis/blob/c686daf450aa58a8c1942785f26c8c2ae7f64d50/Screen%20Shot%202022-07-17%20at%203.29.11%20PM.png" width="500" height="350">

- Balanced Accuracy Score: 0.79
- High Risk Precision Score: 0.03
- Low Risk Precision Score: 1.00
- High Risk Recall Score: 0.70
- Low Risk Recall Score: 0.87

### Easy Ensemble Classifier

<img src="https://github.com/bwheeler98/Credit_Risk_Analysis/blob/c686daf450aa58a8c1942785f26c8c2ae7f64d50/Screen%20Shot%202022-07-17%20at%203.29.22%20PM.png" width="500" height="350">

- Balanced Accuracy Score: 0.93
- High Risk Precision Score: 0.09
- Low Risk Precision Score: 1.00
- High Risk Recall Score: 0.92
- Low Risk Recall Score: 0.94

## Summary

In conclusion each method of sampling produced slightly different results.  To determine which model the business should use, the business would need to clarify what they priortize in order to make this descision.  For example, would they rather catch all of the high risk applications, but have to scipher through them to see if there are any applications that are actually low risk?  Or would they rather catch all of the low risk applications, and face the occassaional actual high risk application that gets passed as low risk.  My recommendation would be to use the Easy Ensemble Classififer method, for the balanced accuracy score was 0.93.
