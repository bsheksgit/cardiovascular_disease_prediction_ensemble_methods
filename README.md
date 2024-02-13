# cardiovascular_disease_prediction_ensemble_methods

* Heart_disease_prediction_EDA.ipynb -> Contains the EDA for the CVD dataset. Univariate, bivariate and multivariate analysis for cardiovascular issues.

* Feature_Engineering_Heart_Diseases.ipynb -> Contains the code for feature engineering for the CVD dataset. 

* Ensemble_methods_Heart_diseases -> Prediction of heart diseases using Ensemble methods like stacking, XGboost and Random Forests.

* Fields in the CVD_cleaned.csv dataset:

General_Health, Chekup, Exercise, Heart_Disease, Skin_Cancer, Other_Cancer, Depression, Diabetes, Arthritis, Sex, Age_Category, Height_(cm), Weight_(Kg), BMI, Smoking_History, Alcohol_Consumption, Fruit_Consumption, Green_Vegetables, FriedPotato_Consumption

* Modified fields in Modified_inputs_targets.csv:

General_Health	Age_Category	Weight_(kg)	Checkup_Never	Checkup_Within the past 2 years	Checkup_Within the past 5 years	Checkup_Within the past year	Exercise_Yes	Skin_Cancer_Yes	Other_Cancer_Yes	Depression_Yes	Diabetes_No, pre-diabetes or borderline diabetes	Diabetes_Yes	Diabetes_Yes, but female told only during pregnancy	Arthritis_Yes	Sex_Male	Height_(cm)_short	Height_(cm)_tall	Height_(cm)_very_tall	BMI_25+_Yes	Smoking_History_Yes	Heart_Disease	Alcohol-Fruit ratio	Fruit-Green ratio	Alcohol-Potato product

EDA is performed with Univariate, Bivariate and Multivariate analysis in Jupyter notebook using matplotlib and seaborn.

Feature engineering is performed for the entire dataset to clean it for making it suitable for the algorithm. 

One hot encoding is done to the categorical columns.

Scaling is done for the numerical columns.

Results:

Feature engineering notebook creates two csv files. Both have different types of feature engineering. Same models are created for both datasets. Score is mentioned for the first dataset.

•	Then data is split into train and test sets. 80% is for training and 20% is for test. Both sets are scaled using standard scaler.

•	3 ensemble models are used to create models, Stacked model, XGboost and Random Forests. Stacked model is created using Logistic regression, Decision trees and K nearest neighbors.

•	Accuracy in Stacked model: 0.8637, accuracy in XGboost: 0.9187, accuracy in Random Forests: 0.9134.

