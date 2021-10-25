# Credit_Risk_Analysis

## Overview 

Credit Risk has been studied for last couple of decades to try and stay ahead of it and manage to maintain high-profits and correct reinvestments. In this analysis various different models were designed and trained to take into consideration the factors from the loan_stats csv. For the training of the models in this case a combination of imbalanced-learn and scikit libraries and evaluate them through resampling. 

For the first models, the oversample was made through randomoversampler and SMOTE algorithm with an undersampled data using the clustercentroid algorithm. For the rest there was and under and oversample approach for the data using SMOTEENN algorithm. Finally a comparison between two machine learning models that have as an objective the minimization of bias; the models are balancedrandomforestclassifier and easyensembleclassifier. 

## Results 

- Naive Random Oversampling:
Accuracy: 66.63%
Low positivity: 1%
Recall: 70%
![image](https://user-images.githubusercontent.com/85911181/138756647-0c155338-2683-41dd-9a0d-65328fdce325.png)


- SMOTE
Accuracy: 66.23%
Low positivity: 1%
Recall: 69%
![image](https://user-images.githubusercontent.com/85911181/138756691-4b1cad61-8059-41c5-a1e6-6a8827499f1b.png)


- Undersampling
Accuracy: 66.23%
Low positivity: 1%
Recall: 40%
![image](https://user-images.githubusercontent.com/85911181/138756762-b61f0b86-1882-480e-8643-d9c27ed1f900.png)


- Combined over and under
Accuracy: 54.42%
Low positivity: 1%
Recall: 57%
![image](https://user-images.githubusercontent.com/85911181/138756865-6f5c8da1-9033-49a3-871b-900336791b17.png)

- Balanced Random Forest Classifier
Accuracy: 78.85%
Precision: 99%
Recall: 88%
![image](https://user-images.githubusercontent.com/85911181/138757399-6d12c797-7f32-499d-a513-4586e35ebcbc.png)

- Easy Ensemble AdaBoost Classifier
Accuracy: 91.79%
Precision: 99%
Recall: 94%
![image](https://user-images.githubusercontent.com/85911181/138758675-bb1c7996-de5e-40ee-9b36-e89603b2dc59.png)

## Summary 

The first models were undersampled, oversampled and the combination of both to try and determine which was the best model for the prediction of loans that have high risk. The four of them presented accuracies that were not as high with low recall scores which is not a great indicator for a good and balanced model. The other two models with the resampled data showed better numbers and the Easy Ensemble proved to be the best of all with higher accuracies and recall values and an overall well-balanced model. 
