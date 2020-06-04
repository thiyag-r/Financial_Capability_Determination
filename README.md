# Financial_Capability_Determination
## Objective
The focus of the project is to determine the financial potential of the customers who are capable of repaying the loan to the bank. The leading financial bank is trying to improvise the financial inclusion by providing positive and safe borrowing experience. The solution has to be developed to ensure that clients are capable of repayment are not rejected and thus the bank will be successfully retaining their clients.

## Dataset
The dataset contains 307,497 rows of customers records. The feature target is the one that has to be focussed on. It contains two categories 0 and 1. Here 1 represents the clients who have had difficulties in repayment of loans which means they have made late payments.0 represents the clients are both capable and not capable of paying. Out of this population customers who are actually capable of repaying the loan have to be filtered. There are  totally 37 features in this dataset, 9 features are categorical and rest of them are numerical.

## Exploratory Data Analysis
The dataset was checked for duplicate values and null values. There were neither duplicate nor null values. Except 5 features all other features have different categories or levels. The 5 features that do not have categories are amt_annuity, amt_credit, amt_income_total, days_birth and days_employed. There is one more category in code_gender  feature which is ‘XNA’ but this does not seem to have any impact on the analysis as there are only 4 such customers.

## Modelling
The Dataset was imported into Scala IDE, with the help of spark core technique the data analysed using SQL. As it was difficult to read and understand the thousand of rows in Scala IDE, the data was imported and analysed using PySpark by importing the spark configurations in Jupiter notebook as it was easy to visualize the data. Once the data imported, each individual feature was analysed to determine whether that field contributes to arriving at a decision. After determining the important feature, the category within that feature is analysed for better result. For example, of all the features, Income type is important feature in determining the status of customer. The working-class category of the Income type features has the higher changes of repaying the loan.

## Conclusion
Based on the analysis, the dataset was filtered by important feature such as educational qualification, income type, age, days employed are performed better in finding the result. This gave an output of 79,406 rows of customer record which is 25.8% of the total population of customers is certainly capable of repaying loan.
