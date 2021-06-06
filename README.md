# Credit_Risk_Analysis

## Purpose

In order to deal with the inherently unbalanced classification problems of credit analysis due to the greater number of good loans, we will employ different techniques to train an evaluate models with unbalanced classes.

We will be using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

## Results

### Naive Random Sampling
![naive_random_sampling](https://github.com/jdfiel/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/naive_random_oversampling.png)

* Accuracy:0.60
High-Risk
* Recall:Moderate (0.6)
* Precision: Low (0.1)

Low-Risk
* Recall:Perfect (1.0)
* Precision:Moderate (0.6)


### Oversampling
![SMOTE_oversampling](https://github.com/jdfiel/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/SMOTE_oversampling.png)

* Accuracy:0.64
High-Risk
* Recall:Moderate (0.62)
* Precision: Low (0.1)

Low-Risk
* Recall:Perfect (1.0)
* Precision:Moderate (0.66)

### Undersampling
![SMOTE_undersampling](https://github.com/jdfiel/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/SMOTE_undersampling.png)

* Accuracy:0.53
High-Risk
* Recall:Moderate (0.62)
* Precision: Low (0.1)

Low-Risk
* Recall:Perfect (1.0)
* Precision:Moderate-Low (0.44)

### SMOTEEN
![SMOTEEN](https://github.com/jdfiel/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/SMOTEEN.png)

* Accuracy:0.60
High-Risk
* Recall:Moderate (0.63)
* Precision: Low (0.1)

Low-Risk
* Recall:Perfect (1.0)
* Precision: Moderate (0.57)

### Balanced Random Forest
![brf](https://github.com/jdfiel/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/brf.png)

* Accuracy:0.79
High-Risk
* Recall:Moderate (0.67)
* Precision: Low (0.03)

Low-Risk
* Recall:Perfect (1.0)
* Precision: Moderate (0.91 )
### Easy Ensemble AdaBoost
![adaboost](https://github.com/jdfiel/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/adaboost.png)

* Accuracy:0.90
High-Risk
* Recall:Moderate (0.92)
* Precision: Low (0.09)

Low-Risk
* Recall:Perfect (1.0)
* Precision: Moderate (0.94)

## Summary

Looking at the results it is clear that the ensemble methods heavily out perform the sampling methods. 

Both ensemble methods demonstrated high accuracy. More importantly, both showed high recall scores for both high risk and low risk scores. EasyEnsemble AdaBoost outperformed Balanced Random Forest slightly. It is important to note that both ensemble methods suggest an over fit of the data.

Depending on the goals of the company, it may be OK to use the EEA method. However, further investigation into over fit would be highly recommended.
