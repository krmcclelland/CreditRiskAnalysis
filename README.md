# Credit Risk Analysis
Supervised Machine Learning and Credit Risk

## Overview of the loan prediction risk analysis:   
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques were used to train and evaluate models with unbalanced classes. Various libraries and algorithms were used to build and evaluate models using resampling including: 
* BalancedRandomForestClassifier (bias reduction model)
* ClusterCentroids algorithm
* EasyEnsembleClassifier (bias reduction model)
* imbalanced-learn 
* RandomOverSampler
* scikit-learn
* SMOTE algorithms
* SMOTEENN algorithm

## Purpose: 
* Explaination on machine learning algorithm use in data analytics.
* Create training, test groups, and split from a given data set.
* Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
* Interpret the results of:
  * Logistic regression
  * Decision tree
  * Random forest
  * Support vector machine algorithms.
* Compare the advantages and disadvantages of each supervised learning algorithm.
* Determine with method is the best supervised learning algorithm for the given scenario.
* Use ensemble and resampling techniques to improve model performance.

## Results:
The results for the six (6) machine learning models including their respective balanced accuracy, precision, and recall scores are as follows:      

### Naive Random Oversampling
![Pic 1](https://github.com/krmcclelland/CreditRiskAnalysis/blob/main/Module-17-Challenge-Resources/Images/17-1%20Naive%20Random%20Oversampling.png)     
1. Counter: Low Risk 51,352 / High Risk 51,352
2. Logistic Regression (Random State = 1)
3. Balanced Accuracy: 0.6249984891886339
4. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
5. Recall: High/Low risk = .60/.65

### SMOTE Oversampling
![Pic 2](https://github.com/krmcclelland/CreditRiskAnalysis/blob/main/Module-17-Challenge-Resources/Images/17-2%20SMOTE%20Oversampling.png)     
1. Counter: Low Risk 51,352 / High Risk 51,352
2. Logistic Regression (Random State = 1)
3. Balanced Accuracy: 0.6512584051472337
4. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
5. Recall: High/Low risk = .64/.66

### Undersampling
![Pic 3](https://github.com/krmcclelland/CreditRiskAnalysis/blob/main/Module-17-Challenge-Resources/Images/17-3%20Undersampling.png)     
1. Counter: Low Risk 260 / High Risk 260
2. Logistic Regression (Random State = 78)
3. Balanced Accuracy: 0.6512584051472337
4. Precision:  The precision is low for High-risk loans and is high for Low-risk loans.
5. Recall: High/Low risk = .60/.44

### Combination Over and Under Sampling
![Pic 4](https://github.com/krmcclelland/CreditRiskAnalysis/blob/main/Module-17-Challenge-Resources/Images/17-4%20Combination%20(Over%20and%20Under)%20Sampling.png)     
1. Counter: High Risk 68,460 / Low Risk 62,011)
2. Logistic Regression (Random State = 1)
3. Balanced Accuracy: 0.5161072635781654
4. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
5. Recall: High/Low risk = .70/.57

### Balanced Random Forest Classifier
![Pic 5](https://github.com/krmcclelland/CreditRiskAnalysis/blob/main/Module-17-Challenge-Resources/Images/17-5%20Balanced%20Random%20Forest%20Classifer.png)     
1. Balance Random Forest Classifier (Random State = 1)
2. Balanced Accuracy: 0.7877672625306695
3. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
4. Recall: High/Low risk = .67/.91

### Easy Ensemble AdaBoost Classifier
![Pic 6](https://github.com/krmcclelland/CreditRiskAnalysis/blob/main/Module-17-Challenge-Resources/Images/17-6%20Easy%20Ensemble%20AdaBoost%20Classifier.png)     
1. Easy Ensemble Classifier (n Estimators = 100, Random State = 1)
2. Balanced Accuracy: 0.925427358175101
3. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
4. Recall: High/Low risk = .91/.94

## Summary:
When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model.  
* Credit Card Data Set
  * For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy.  
  * The other models were below .80 balanced accuracy.  
* The precision for all models were similar and within an appropriate range.  The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model.  
* The Easy Ensemble AdaBoost Classifier had the highest recall score, making it the final best machine learning model to choose for further credit card analysis.   
