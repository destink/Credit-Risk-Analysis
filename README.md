# Credit_Risk_Analysis
## Analysis
The purpose of this analysis is to determine which supervised machine learning model will be able to most accurately predict whether a person is high risk or low risk given the variables associate with that person’s financial profile.

The purpose of this analysis is well defined 
## Results:
### Oversampling
* Naive Random Oversampling
  * Accuracy Score: 0.646
  * Precision Score: high_risk = 0.01, low_risk = 1.00, avg = 0.99
  * Recall Score: high_risk = 0.71, low_risk = 0.58, avg = 0.58
# ![](Images/Naive.PNG)
* SMOTE Oversampling
  * Accuracy Score: 0.675
  * Precision Score: high_risk = 0.01, low_risk = 1.00, avg = 0.99
  * Recall Score: high_risk = 0.66, low_risk = 0.69, avg = 0.69
# ![](Images/Smote.PNG)
### Undersampling
* Cluster Centroids Undersampling
  * Accuracy Score: 0.544
  * Precision Score: high_risk = 0.01, low_risk = 1.00, avg = 0.99
  * Recall Score: high_risk = 0.69, low_risk = 0.40, avg = 0.40
# ![](Images/Cluster_Centroids.PNG)
### Combination (Over/Under) Sampling
* Smoteenn Combination Sampling
  * Accuracy Score: 0.666
  * Precision Score: high_risk = 0.01, low_risk = 1.00, avg = 0.99
  * Recall Score: high_risk = 0.73, low_risk = 0.60, avg = 0.60
# ![](Images/Smoteenn.PNG)
### Ensemble Learners 
* Balanced Random Forest Classifier
  * Accuracy Score: 0.789
  * Precision Score: high_risk = 0.03, low_risk = 1.00, avg = 0.99
  * Recall Score: high_risk = 0.70, low_risk = 0.87, avg = 0.87
# ![Balanced_Random_Forest_ Classifier](https://user-images.githubusercontent.com/95573310/222475287-1e3afb4b-243e-4b8a-bf36-9889f3624908.PNG)
* AdaBoost Classifier
  * Accuracy Score: 0.688
  * Precision Score: high_risk = 0.88, low_risk = 1.00, avg = 1.00
  * Recall Score: high_risk = 0.38, low_risk = 1.00, avg = 1.00
# ![](Images/AdaBoost.PNG)

## Summary:
The model that displayed the highest levels of accuracy and precision is the ensemble learner, balanced random forest classifier model with 0.789 and an avg of 0.99, respectively for the entire population. The accuracy of this model is what really sets it apart from the rest of the models. However, the adaboost classifier provided the highest precision score by a huge margin of the high-risk population. Which is really the metric that a credit risk analysts would be concerned with. This model’s accuracy is acceptable compared to the other five models and although the recall score is only at 0.38, the proportion of which positive identifications was correct, the precision of 0.87, of high risk, is by far the most accurate at determining the proportion of positive identifications that were correct.  The only other model that had a higher recall for high risk of 0.01 was the other ensemble learner model, balanced random forest classifier at 0.03. In summary, for this analysis using the adaboost classifier model is the most reliable model with this data set. 
