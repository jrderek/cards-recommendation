# Credit-Card-Default-Analysis
Model to predict whether customer default on loan or not
The purpose of this project is to conduct quantitative analysis on credit card default risk by using 3 machine learning models with accessible customer data, instead of credit score or credit history, with the goal of assisting and speeding up the human decision making process.
# Project Overview
The analysis consists of 2 Jupyter notebooks.

Exploratory Data Analysis. The detailed notebook of EDA can be found here.
Machine Learning Modeling. The detailed notebook of modeling can be found here.
Machine Learning Models Used:

Logistic Regression
Random Forest
XGBoost
See the [presentation slides](https://github.com/AnshRockstar/Credit-Card-Default-Analysis/blob/main/Credit-Card-Default-Prediction.pptx) for a summary of this analysis.

# Key Findings from EDA
1.Males have more delayed payment than females in this dataset. Keep in mind that this finding only applies to this dataset, it does not imply this is true for other datasets.\
2.Customers with higher education have less default payments and higher credit limits.\
3.Customers aged between 30-50 have the lowest delayed payment rate, while younger groups (20-30) and older groups (50-70) all have higher delayed payment rates. However, the delayed rate drops slightly again in customers older than 70.\
4.There appears to be no correlation between default payment and marital status.\
5.Customers being inactive doesn’t mean they have no default risk. We found 317 out of 870 inactive customers who had no consumption in 6 months then defaulted next month.



# Model Comparison
In these 3 models, Logistic Regression model has the highest recall but the lowest precision, if the firm expects high recall, then this model is the best candidate. If the balance of recall and precision is the most important metric, then Random Forest is the ideal model. Since Random Forest has slightly lower recall but much higher precision than Logistic Regression, we recommend the Random Forest model.

![download](https://user-images.githubusercontent.com/86865912/153705551-fa210ef2-c18f-4631-8e4f-04a5ebe6269b.png)

# Limitations
1.Best model Random Forest can only detect 51% of default.\
2.Model can only be served as an aid in decision making instead of replacing human decision.\
3.Used only 30,000 records and not from US consumers.


# Future Work
1.Models are not exhaustive. Other models could perform better.\
2.Get more computational resources to tune XGBoost parameters.\
3.Acquire US customer data and more useful features.I.e.customer income.
