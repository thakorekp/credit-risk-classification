# credit-risk-classification
Module 20 Challenge

Credit Risk Analysis Report

The purpose of this analysis is to evaluate a Logistic Regression model that is trained on historical lending data from a lending services company to ultimately identify loans in healthy or potentially high risk of default status. The features used in the model include loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. Loan status was classified as '0' for a healthy loan or '1' for a high risk loan. We first read in the raw data from a csv file to a DataFrame, and then separate the y variable or labels, from the X variable or features. We then split the data into training and testing datasets using the train_test_split module. We then create the Logistic Regression model and fit the training data set to it. We then made predictions from the testing feature data and the fitted model, and then generated the confusion matrix and classification report to evaluate the model.

Based on the balanced accuracy score evaluation of the model, we can tell that the model predicted the correct label about 94 percent of the time. From the confusion matrix and classification report, we can see that the model predicted loan status with 99.2% accuracy. The precision of 0.87 tells us what proportion of all high risk classifications were actually correct, taking into account the false positives(false high risk classifications). The recall of 0.89 tells us what proportion of true high risk loan classifications were correctly identified, taking into account false negatives(false healthy loan classifications). Based upon this, I would recommend the model to predict credit risk for customers of this establishment. 

The second model fit with oversampled data had an accuracy of 99%. The precision and recall, as described above, were both 0.99 (higher) with the second model. Based upon this, I would recommend this model fit with the oversampled data over the previous model to predict credit risk more accurately.





Websites used for research:
https://imbalanced-learn.org/stable/over_sampling.html
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.balanced_accuracy_score.html
