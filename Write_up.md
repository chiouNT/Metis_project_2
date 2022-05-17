write_up (Ni-Ting Chiou)

# Linear regression project: Modeling the housing data in the Bay Area

## Abstract

The goal of the project was to use linear regression models to predict the housing prices listed at Zillow website. I scraped 1 target and 8 features from Zillow website.  The categorical features were transformed to dummy variables followed by OLS model fitting. The fitting results showed that most features that have the low correlation to the prices have the coefficients with low significant. After removing these features, and model was further optimized by Lasso regularization. The final model has 7 features and MAE of $ 267,678.


## Data

The raw dataset contains 1097 house prices with 8 features, 2 of which are categorical features. During the data clean processes, null values were removed and 2 categorical features were converted into the dummy variables. Thus, the final dataset contains 620 house prices with 13 features.
  
## Algorithms

*Feature Engineering*
1.	Converting the years of the houses to the age of the houses.
2.	Converting the categorical features to binary dummy variables.
3.	Square-transform the age of the houses.

*Models* <br> 

OLS regression was used for the feature selection and Lasso regularization was used for the final optimalization.
* Final Lasso Model 5-fold CV scores:
0.632
* Train-set scores:
0.646
* test-set scores:
0.644



## Tools
* Numpy and Pandas for data manipulation
* Statsmodel and Scikit-learn for modeling
* Matplotlib and Seaborn for plotting



## Communication
* For the final housing prices model, the important features are sizes and the location of San Jose. For an estimated house prices, it is 1.2 million plus 0.4 million per sqrt of sizes and minus 0.12 million for the location of San Jose. The following figures showed the coefficients of other features.

![alt text](https://github.com/chiouNT/Linear_regression/blob/main/Images/Final_model.png)
