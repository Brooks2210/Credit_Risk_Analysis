# Credit Risk Analysis

## Overview

For the following analysis, my team was tasked with using several supervised machine learning techniques to determine if they were useful in predicting loan risk. Using the credit card dataset from Lending Club, a peer-to-peer lending services company, we oversampled the data using the Random Over Sampler and SMOTE algorithms, and under sampled the data using the Cluster Centroids algorithm. Then, we used a combination approach of over- and under sampling using the SMOTEENN algorithm. Finally, we compared two new machine learning models that reduce bias, the balanced random forest classifier, and the easy ensemble classifier.  

### Resources
Applications: Python, Jupyter Notebook, Scikit-learn, and imbalanced-learn <br/>

### Detailed Results

![RandomOverSample](https://github.com/Brooks2210/Credit_Risk_Analysis/blob/main/Resources/RandomOverSample.png)
- Balance Accuracy Score: 0.6770
- Precision: .99
- Recall/Sensitivity: .59
- F1: .74

![SMOTE](https://github.com/Brooks2210/Credit_Risk_Analysis/blob/main/Resources/SMOTE.png)
- Balance Accuracy Score: 0.6624
- Precision: .99
- Recall/Sensitivity: .69
- F1: .81

![Undersampling](https://github.com/Brooks2210/Credit_Risk_Analysis/blob/main/Resources/Undersampling.png)
- Balance Accuracy Score: 0.5447
- Precision: .99
- Recall/Sensitivity: .40
- F1: .56

![Combo](https://github.com/Brooks2210/Credit_Risk_Analysis/blob/main/Resources/Combo.png)
- Balance Accuracy Score: 0.6489
- Precision: .99
- Recall/Sensitivity: .60
- F1: .74

![Balancedrandomforest](https://github.com/Brooks2210/Credit_Risk_Analysis/blob/main/Resources/Balancedrandomforest.png)
- Balance Accuracy Score: 0.7888
- Precision: .99
- Recall/Sensitivity: .87
- F1: .93

![Easyensembleclassifier](https://github.com/Brooks2210/Credit_Risk_Analysis/blob/main/Resources/Easyensembleclassifier.png)
- Balance Accuracy Score: 0.7888
- Precision: .99
- Recall/Sensitivity: .87
- F1: .93

## Summary

The results of the machine models can be seen above, but the initial analysis shows that all six of the models did a poor job of predicting high risk loan applicants. Now on the surface that seems to reflect poorly on the models, but it needs to be put into context. The vast majority (99.5%) of the loan applications came from low-risk applicants. In identifying low-risk applicants, both the balanced random forest and easy ensemble classifiers did well with 100% precision and 87% recall. The highest total F1 score was .93 and both the balanced random forest and easy ensemble classifiers attained that score.

While all the models could use adjustment both the balanced random forest and easy ensemble classifiers could be a helpful tool for our client.  
