# Title of Project: Bank Customer Churn Model

## Objective

The objective of the project is to develop a predictive model that can accurately identify and predict which customers are likely to churn (leave) the bank's services.

![Churn-analysis-by-47Billion](https://github.com/Mohamed-Ashif/Bank-Customer-Churn-Model/assets/78372127/06c33c73-e648-47a5-9424-ff00414adb27)

## Datasource

Bank Customer Churn (https://github.com/YBI-Foundation/Dataset/raw/main/Bank%20Churn%20Modelling.csv) 13 columns, 10,000 rows

◉ CustomerId: Contains random values and has no effect on customer leaving the bank.

◉ Surname: The surname of a customer has no impact on their decision to leave the bank.

◉ CreditScore: Can have an effect on customer churn, since a customer with a higher credit score is less likely to leave the bank.

◉ Geography: A customer’s location can affect their decision to leave the bank.

◉ Gender: It’s interesting to explore whether gender plays a role in a customer leaving the bank.

◉ Age: This is certainly relevant, since older customers are less likely to leave their bank than younger ones.

◉ Tenure: Refers to the number of years that the customer has been a client of the bank. Normally, older clients are more loyal and less likely to leave a bank.

◉ Balance: Also a very good indicator of customer churn, as people with a higher balance in their accounts are less likely to leave the bank compared to those with lower balances.

◉ Num Of Products: Refers to the number of products that a customer has purchased through the bank.

◉ Has Credit Card: Denotes whether or not a customer has a credit card. This column is also relevant, since people with a credit card are less likely to leave the bank.

◉ Is Active Member: Active customers are less likely to leave the bank.

◉ Estimated Salary: As with balance, people with lower salaries are more likely to leave the bank compared to those with higher salaries.

◉ Churn: Whether or not the customer left the bank.

## Explaination

In order to create a model these are the following procedure -

Split the dataset in 70% of Train set and 30% of Test Set.

Feature engineering.

Handling Imbalanced Data.

Check the accuracy score for both Training and Test Set.

Compare the accuracies for both Training and Test set, in order to check for the overfitting issues.

## Conclusion

Finally, Using Random Over Sampling technique with Random Forest Classifier Model [Fine Tuned] has achieved a highest accuracy of 91%.

