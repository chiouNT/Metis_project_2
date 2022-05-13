Minimum Viable Product (Ni-Ting Chiou)

##  Model of Zillow house prices

* **Numeric feature selection:** The features, bathrooms and school-ratings, have the no-significant coefficents. When these 2 features are removed, the R2 of test dataset is still 0.54.

* **Addition of the categorical features:** The categorial features,hometypes and citys, are added for modeling. When the categorical features are added, the R2 is increased from 0.54 to 0.652.

* **Regularization:** When Lasso regularization is performed, R2 of the test dataset is reduced from 0.653 to 0.652.


* **Results:** The following results showed that the factor of sizes is more important than the factor of room numbers.
![alt text](https://github.com/chiouNT/Linear_regression/blob/main/Images/Model_evaluation.png)

![alt text](https://github.com/chiouNT/Linear_regression/blob/main/Images/Feature%20comparison.png)


