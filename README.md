LOAN DEFAULT PREDICTION ANALYSIS

The purpose of this analysis is to develop machine learning models to predict loan defaults for a lending company. The goal is to provide accurate predictions to identify loans that have a high risk of defaulting. Two models were used in this analysis: logistic regression model with original data and logistic regression with oversampled data.

results:
Logistic regression model(original)
1.balanced accuracy score is 0.9521.
2.confusion matrix 
[[14926    75]
 [   46   461]]
3.classification report:
              precision    recall  f1-score   support

         0       1.00      1.00      1.00     15001
         1       0.86      0.91      0.88       507

  accuracy                           0.99     15508
 macro avg       0.93      0.95      0.94     15508
weighted avg 0.99 0.99 0.99 15508

logistic regression model2 (oversampled)
1.balanced accuracy score is 0.9942
2.confsion matrix:
[[14915 86]
[ 3 504]]
3.classification report:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     15001
           1       0.85      0.99      0.92       507

    accuracy                           0.99     15508
   macro avg       0.93      0.99      0.96     15508
weighted avg       1.00      0.99      0.99     15508


Both machine learning models, logistic regression with the original data and logistic regression with oversampled data, demonstrated strong predictive performance in predicting loan defaults.

The logistic regression model with the original data achieved a balanced accuracy score of 0.9521. It accurately predicted healthy loans with high precision and recall, achieving an F1-score of 1.00. For high-risk loans, it had a slightly lower precision but still achieved a good recall and F1-score.

On the other hand, the logistic regression model with oversampled data achieved a significantly higher balanced accuracy score of 0.9942. It accurately predicted both healthy loans and high-risk loans with high precision, recall, and F1-scores. It demonstrated a good balance between precision and recall for high-risk loans, even though there were a few false positives.

Considering the excellent performance of the logistic regression model with oversampled data, it is recommended for use by the lending company. This model achieves a very high balanced accuracy score and accurately predicts loan defaults for both healthy loans and high-risk loans. By utilizing oversampled data, the model is better able to capture the patterns and characteristics of high-risk loans, resulting in improved predictive performance.

However, it is important to note that this recommendation is based solely on the performance of the models. Other factors, such as computational resources and implementation considerations, should also be taken into account before finalizing the choice of model for production use.
