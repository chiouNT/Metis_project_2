write_up (Ni-Ting Chiou)

# Linear regression project: Modeling the housing data in the Bay Area

## Abstract

The goal of the project was to use linear regression models to predict the housing prices listed at Zillow website. I scraped 1 target and 8 features from Zillow website.  After feature engineering, the correlation anaylsis and OLS model fitting were performed. It showed that the features having low correlation to the targets usually have the coefficients with low significant. After removing these features, and model was further optimized by Lasso regularization. The final model has the constant of 1.2 million and MAE of 0.28 million.

## Design

To predict the listed house prices, the listed prices and features were scraped from Zillow websites. 8 features were scraped. For numeric features, they include sizes, number of bedrooms, bathrooms and garages, year built and school rating. For categorical featuers, they include city and hometypes.

## Data

The raw dataset contains 1097 house prices with 8 features. During the data clean processes, null values were removed and 2 categorical features were converted into the dummy variables. Thus, the final dataset contains 620 house prices with 13 features.
  
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
