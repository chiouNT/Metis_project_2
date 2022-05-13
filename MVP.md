Minimum Viable Product (Ni-Ting Chiou)

##  Model of house prices from Zillow websites

* **Numeric feature selection:** The features, bathrooms and school-ratings, have the no-significant coefficents.  When these 2 features are removed, the R2 of train vs test dataset is still 0.54 and 0.56.

* **Addition of the categorical features:** The categorial features,hometypes and citys, are added for modeling. When the categorical features are added, the R2 of train vs test dataset is 0.64 and 0.65.

* **Regularization:** When Lasso regularization is performed, the R2 of train vs test dataset is 0.64 and 0.66.


##  Predictions of house prices

* **Model_evaluation:** 

![alt text](https://github.com/chiouNT/Linear_regression/blob/main/Images/Model_evaluation.png)


* **Feature comparison:** 

![alt text](https://github.com/chiouNT/Linear_regression/blob/main/Images/Feature%20comparison.png)


