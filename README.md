# Credit Risk Analysis
In this project were created Linear regression model and Ensemble Classifiers to predict loan risk. 

## Linear Regression
As the data sample was unbalanced (we had much more low risks application than high risk) were conducted four resampling models: Naive Random Oversampling, SMOTE Oversampling, Cluster Centriod Undersampling and SMOTEENN approach (written analysis of each conducted model could be found in the code body)

### Best Linear regression model
All four models showed precision equal or close to one, so all or almost all applications that were classified as low risk were actually low risk. However SMOTE oversampling model showed the highest recall for low risk applications (67%). It means that 67% of actually low risk cases were classified as low risk and might be approved. Although the accuracy of this model is only the second highest among other models (64%), given the better recall performance this model might be recommended for preliminary evaluation of applications.

## Ensemble Classifiers
Additionally were conducted two ensemble classifiers: Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier. Although both models have precise of low risk equal to 1, Adaboost Classifier has higher accuracy then Balanced Random Forest Classifier (93% vs. 75%) and higher recall (94% vs 88%).
It means that using Adaboost Classifier model 100% of predicted low risk applications were actually low risk and 94% of all actual low risk applications were predicted by this model. 
This model might be successfully used to predict low risks applications.
