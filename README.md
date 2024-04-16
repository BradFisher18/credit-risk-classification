# credit-risk-classification
Repository for Module 20 - Supervised Learning
## Overview of the Analysis
In this analysis, we are using linear regression to assist the lending services company identify which loans are high-risk. \
This model utilises the provided persons loan and income data including; loan amount, interest rate, their income, debt to income rate, numberr of accounts, derogatory marks, and total debt.\
To complete this analysis, the loan status was first isolated and saved as its own variable 'y', while the remaining data columns were saved as the main features impacting the riskiness of the loan. The variable 'y' and the features were then split into training and testing lists. The training data is used based on existing loan status so that trhe model can learn and understand the influenece of the features has. Once the models training has completed, it then tests it on the testing data and we can then se those results and compare it to the actuial results to determine if this model if effective and may be used going forward.\
The logistic Regression model itself is a statistical method for predicting binary outcomes, in this case determining if the loan is healthy (0) or high-risk (1). Using the sigmoid function, converts the continuous data to a percentage, and depending on the threshold for classification it is then translated to be 0 or 1. 
## Results
* ACCURACY: This model was found to be very accurate. Due to the dataset being very imbalanced with the vast majority of persons having a healthy loan, the weighted average accuracy is a better representation, in which this models achieves 0.99 for both.
* PRECISION: This model acieves a precision of 1.00 for loans deemed as healthy, however for high risk it only achieves 0.85. As this model is only flagging high-risk loans, the impact of low precision is of minimal impact, particularly when we consider the size of the dataset being true positive.
* RECALL: This model achieved a recall of 0.99 and 0.91 for negative and positive respectively. The recall for negative can be explained by the sample size of negative values within the dataset, meaning that any false does not have a great impact on this value. Comparitively, as the amount of positive values is significantly less, the recall rate of 0.91 is good as it is saying within the limited number of actual number of positive instances, it was able to identify it at a high rate. 

## Summary
Overall, this model is very effective and is recommended for use by the company.\
The model achieves good scores in aspect of the classification report, with all values achieving within the 0.9's with the exception of positive precision achieving 0.85. Given how vastly imbalanced the datset is between actual negative and positive values (18,765 versus 619), this further solidifies that the accuracy, precision and recall rates are acceptable. When we also consider that the impact of a false negative will not have a direct impact on the person or business, this again indicates this model is suitable for use
