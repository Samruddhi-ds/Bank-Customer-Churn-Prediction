# Bank-Customer-Churn-Prediction

## Problem Statement
This data set contains details of a bank's customers and the target variable is a binary variable reflecting the fact whether the customer left the bank (closed his account) or he continues to be a customer. We have to build a model to predict that on the basis of the customer attributes, will customer leave the bank or stay.


1.Requires Jupyter Notebook to run the following file 
2.Proper Libraries to be installed
3.Data Dictionary
* RowNumber: Row Numbers from 1 to 10000
* CustomerId: Unique Ids for bank customer identification
* Surname: Customer's last name
* CreditScore: Credit score of the customer
* Geography: The country from which the customer belongs
* Gender: Male or Female
* Age: Age of the customer
* Tenure: Number of years for which the customer has been with the bank
* Balance: Bank balance of the customer
* NumOfProducts: Number of bank products the customer is utilising
* HasCrCard: Binary Flag for whether the customer holds a credit card with the bank or not
* IsActiveMember: Binary Flag for whether the customer is an active member with the bank or not
* EstimatedSalary: Estimated salary of the customer in Dollars
* Exited: Binary flag 1 if the customer closed account with bank and 0 if the customer is retained

Target Column Description: Exited is a class label used to divide into groups (customer closed account or not).

4.Started with basic Exploratory Data Analysis
* Plotted Bar Chart for Categorical Variables

![image](https://user-images.githubusercontent.com/78426725/115423360-5fccb500-a21b-11eb-9d76-9dd614d4577a.png)
![image](https://user-images.githubusercontent.com/78426725/115423400-6a874a00-a21b-11eb-9a5e-392ee3464961.png)
![image](https://user-images.githubusercontent.com/78426725/115423438-71ae5800-a21b-11eb-8a23-fcf2d5f18526.png)
![image](https://user-images.githubusercontent.com/78426725/115423467-796dfc80-a21b-11eb-8b6d-5ca100221cd2.png)



* Insights Drawn from Charts
	-We have 50 % of data of France followed by Germany and spain
	-We have 54 % Data of males and 45 % of females
	-70% people have credit card and 30% don't have it
	-51% people are active members in our data.

5.Checked for the Data imbalanceness in the data and dealt with the same using SMOTE

  ![image](https://user-images.githubusercontent.com/78426725/115423569-90145380-a21b-11eb-8e08-2f6703fac640.png)


6.Basic Model Building 
	-Logistic Regression using Logit to get the significance of the unbalanced Data as well as Balanced Data
	-Accuracy decreased by approx 2% in SMOTE but this was ok as there is resampling done using SMOTE to balance the data
7.Using Different Classification Models.
	-Decision Tree Classifier with and without Hyperparameter tuning
	-Hyperparameter Tuning gave better results and fitted well on the test data as well.
  
  ![image](https://user-images.githubusercontent.com/78426725/115423772-b934e400-a21b-11eb-9cd2-49f0c8d0f6eb.png)


8.Risk in Banking Churn is the SMOTE Analysis may have created an error in the data as we have added the data in it without knowing the actual values.
