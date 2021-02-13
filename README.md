
# Supervised Learning: Bank Lending Algorithm

[**Dataset**](https://www.kaggle.com/kennykozak/loan-repayment-prediction?select=loan_data_final.csv)

This project will analyze what factors are most important in securing a loan. The records are applications to LendingClub.com for all types of loans (personal, debt consolidation, educational and small business). Applicants are analyzed for certain criteria according to LendingClub.com's standards.

The objective is to see if it is possible to recreate a lending algorithm for peer-to-peer lending or mircolending.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/13NUEak9fC4cPd7rf1I9DcMHAF5zHOU3f/view?usp=sharing)


----

## Key Features

![image](https://storage.googleapis.com/lending_algorithm/corr_chart.png)
![image](https://storage.googleapis.com/lending_algorithm/feature_importances.png)
![image](https://storage.googleapis.com/lending_algorithm/FICO-dist.png)


- Notes
	* 19.5% unapproved, 80.5% approved
	* FICO, revolving credit balance and interest rates were the most highly correlated with loan approval

----

## Integrations

* [GridSearch](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)
* [RandomForest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
* [GradientBoostingRegressor](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingRegressor.html)
* [DecisionTreeClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)

----

## Conclusions

![image](https://storage.googleapis.com/lending_algorithm/r_forest_conf_matrix.png)

The best results came from the random forest classifier with parameters optimized by GridSearch. This had the highest recall on the minority class at 92%.

|	   |precision| recall|	f1-score|support|
| -------- | ------ | ----- | ----- | -------- |
|**unapproved**|	0.99|	0.92|	0.95|	372.0|
|**approved**|	0.98|	1.0|	0.99|	1,544.0|
|**accuracy**|	0.98|	0.98|	0.98|	0.98|
|**macro avg**|	0.98|	0.96|	0.97|	1,916.0|
|**weighted avg**|	0.98|	0.98|	0.98|	1,916.0|


----

## Questions/Comments

Any contributions are more than welcome!

Feel free to leave me a message on Git or email me at mcclure.dean@gmail.com
