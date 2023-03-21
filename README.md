# Module_12

## Overview of Analysis
* Purpose of this analysis was to find a technique that helped identify the credit worthiness of the borrowers by training and evaluating models with imbalanced classes. 
* The financial information was lending data with multiple columns but the most important information that was going to be used in the models was "loan_status". What I needed to predict was how effective a logistic regression model is predicting boh healthy loan and high-risk loan labels by using the loan_status column to train the model. I also used a RandomOverSampler module to resample the data to fit the model and make some new predictions. After completion I compared both methods to determine which was more effective. 
* The values used in "loan_status" was 0 (Healthy Loan) and 1 (High-Risk loan)
* The stages in the machine learning processes began with creating a logistic regression model using the original data. Once that was completed I went on to evaluating the models performance by calculating the accuracy score of the model, generating a confusion matrixs and then printing a classification report. I repeated that processes again but before I started the process I imported the RandomOverSapler and fit the original training data to the random_oversampler model. 

## Results
* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

* Accuracy: 0.9520479254722232

                    pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.99      0.91      1.00      0.95      0.91     18765
          1       0.85      0.91      0.99      0.88      0.95      0.90       619
avg / total       0.99      0.99      0.91      0.99      0.95      0.91     19384

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

* Accuracy: 0.9936781215845847

                   pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.99      0.99      1.00      0.99      0.99     18765
          1       0.84      0.99      0.99      0.91      0.99      0.99       619
avg / total       0.99      0.99      0.99      0.99      0.99      0.99     19384



## Summary
Overall I personally think that the Logistic Regression model using RandomOverSampler module to resample the data was a more effective model than without the resampled data. From the data that I gathered we can see that the resampled data is more accurate than when the data was not resampled. The closer to 1 each column is the more accurate the model is and since the resampled data is closes to 1 I believe it is the winner in this. The data used in logisitc regression is specificly tailored to 0 and 1 data and neither 0 or 1 is more important. Overall I would use the resampled data with a logisitic regression model. 