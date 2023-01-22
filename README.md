![Surviving-a-Credit-Card-Default](https://user-images.githubusercontent.com/60965420/205428396-f01f1512-733d-42b2-9ffd-edd6c33b0af8.png)
# Credit Card Default Prediction
This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. We can use the K-S chart to evaluate which customer will default on their credit card payments.
# **Dataset Information**
* **Number of instances: 30000**
* **Number of attributes: 25**
# **Features Information**

* **ID:** ID of each client

* **LIMIT_BAL**: Amount of given credit in NT dollars (includes individual and family/supplementary credit)

* **SEX**: Gender (1 = male, 2 = female)

* **EDUCATION**: (1 = graduate school, 2 = university, 3 = high school, 0,4,5,6 = others)

* **MARRIAGE**: Marital status (0 = others, 1 = married, 2 = single, 3 = others)

* **AGE**: Age in years

* **Scale for PAY_0 to PAY_6 :** (-2 = No consumption, -1 = paid in full, 0 = use of revolving credit (paid minimum only), 1 = payment delay for one month, 2 = payment delay for two months, ... 8 = payment delay for eight months, 9 = payment delay for nine months and above)

* **PAY_0**: Repayment status in September, 2005 (scale same as above)

* **PAY_2**: Repayment status in August, 2005 (scale same as above)

* **PAY_3**: Repayment status in July, 2005 (scale same as above)

* **PAY_4**: Repayment status in June, 2005 (scale same as above)

* **PAY_5**: Repayment status in May, 2005 (scale same as above)

* **PAY_6**: Repayment status in April, 2005 (scale same as above)

* **BILL_AMT1:** Amount of bill statement in September, 2005 (NT dollar)

* **BILL_AMT2:** Amount of bill statement in August, 2005 (NT dollar)

* **BILL_AMT3:** Amount of bill statement in July, 2005 (NT dollar)

* **BILL_AMT4:** Amount of bill statement in June, 2005 (NT dollar)

* **BILL_AMT5:** Amount of bill statement in May, 2005 (NT dollar)

* **BILL_AMT6:** Amount of bill statement in April, 2005 (NT dollar)

* **PAY_AMT1:** Amount of previous payment in September, 2005 (NT dollar)

* **PAY_AMT2:** Amount of previous payment in August, 2005 (NT dollar)

* **PAY_AMT3:** Amount of previous payment in July, 2005 (NT dollar)

* **PAY_AMT4:** Amount of previous payment in June, 2005 (NT dollar)

* **PAY_AMT5:** Amount of previous payment in May, 2005 (NT dollar)

* **PAY_AMT6:** Amount of previous payment in April, 2005 (NT dollar)
# **Target Variable**
* **default payment next month:** 1-Default, 0-Not default
# **Goal**

The main objective of our project is to predict which customer might default in upcoming months.

**Meaning:**
* We are all aware what is credit card. It is type of payment payment card in which charges are made against a line of credit instead of the account holder's cash deposits. When someone uses a credit card to make a purchase, that person's account accrues a balance that must be paid off each month.

* Credit card default happens when you have become severely delinquent on your credit card payments.Missing credit card payments once or twice does not count as a default. A payment default occurs when you fail to pay the Minimum Amount Due on the credit card for a few consecutive months.
# **Prerequisites**
* Understanding of ML algorithms
# **Technologies used**
* IDE- Google colab
# **Project Work flow**
1. Importing Libraries

2. Loading the Dataset

3. EDA on features

4. Feature Engineering

5. Feature Selection

6. Modeling and HyperParameter Tuning

7. Selecting the best model

8. Conclusion

# **Conclusion**
Started with loading the data so far we have done EDA ,feature engineering , one hot encoding of categorical columns, feature selection and then model building. So far we have modelled on

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier


After hyper parameter tuning, we have prevented overfitting and decreased errors.

Out of all these models RandomForestRegressor is the best performer in terms of f1-score.

The strongest predictors of default are the PAY_AMTX, the LIMIT_BAL & the BILL_AMT_X, PAY_X, AGE and SEX on the basis of models used.

Using a Logistic Regression classifier, we can predict with ~60% accuracy, whether a customer is likely to default next month.

Using a Decision Tree classifier, we can predict with ~76% accuracy, whether a customer is likely to default next month.

Using a Random Forest classifier, we can predict with ~85% accuracy, whether a customer is likely to default next month.

It mean out of 100 defaulters 85 will be correctly caught by Random Forest Classifier.

**Demographics:** We see that being Female, More educated, Single and between 30-40 years old means a customer is more likely to make payments on time.

![16141199232018](https://user-images.githubusercontent.com/60965420/213905676-1e5e0de6-14de-49fe-81eb-9e68238b1fe5.png)

