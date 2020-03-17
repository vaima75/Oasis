## Tele-Marketing Sales Prediction: Classification Problem

This case-study was given by [Desicison Point](http://decisionpoint.in/)

### Case-Study : Oasis  Problem Statement

Company X relies upon telemarketing to sell products.

Your project lead wants to utilize the opportunity and prepare a business development case for predictive modeling assignment. The lead has asked you to explore different available techniques and prepare a few slides on the technique which can be implemented on the business. The lead has also requested you to prepare the objective of the model, list additional data requirement and briefly describe the model- include steps and possible impact on the business.

The column headers are self-explanatory, with the 'Sale' column indicating whether a sale was made or not when Agent X called the customer.

#### Data Description
| Sno | Variables | Description |
|----|----|----|
| 1 | Call_ID | Customer Call ID|
| 2 | Sale | Did Sale Happend? |
| 3 | Agent_ID | ID of Agent |
| 4 | Age | Age of Customer |
| 5 | Product_ID | ID of Product |
| 6 | Timezone | Timezone where call was made |
| 7 | Phone_code | Customer's Phone Code |
| 8 | First_Name | Customer's First Name |
| 9 | Last_Name | Customer's First Name |
| 10 | Area_Code | Location Code of Customer |
| 11 | Gender | Customer's Gender |
| 12 | Call_Count | Calls made to customer by Agent X |


### Methodology

* Data - Preprocessing
	- Feature Creation and Preparation
	- Outlier Treatment
	- Imputation Method

* Model Preparation and Algorithms
	- Sampling Techniques
		+ Over sampling
		+ SMOTE
		+ SMOTE Tomek 
	- Modelling Algorithms
		+ Random Forest
		+ XGBOOST

### Results

| Mno | Model | Sampling Method | Accuracy | F1 Score | Recall | ROC-AUC | PR-AUC |
|----|----|----|----|----|----|----|----|
| 1 | RF | Upsample | 0.892 | 0.105 | 0.071 | 0.522 | 0.180 |
| 2 | RF | SMOTE | 0.901 | 0.071 | 0.040 | 0.514 | 0.175 |
| 3 | RF | SMOTE Tomek | 0.901 | 0.069 | 0.041 | 0.513 | 0.174 |
| 4 | XGBOOST | Upsample | 0.618 | 0.189 | 0.495 | 0.562 | 0.328 |
| 5 | XGBOOST | SMOTE | 0.909 | 0.030 | 0.016 | 0.506 | 0.213 |
| 6 | XGBOOST | SMOTE Tomek | 0.909 | 0.030 | 0.016 | 0.506 | 0.213 |
