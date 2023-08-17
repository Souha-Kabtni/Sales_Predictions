<img width="560" alt="image" src="https://github.com/Souha-Kabtni/Sales_Predictions/assets/133057039/841e91c3-b7b9-4805-bb62-bcf28f5da21a">

A sales prediction for food items sold at various stores. The goal of this is to help the retailer understand the properties of products and outlets that play crucial roles in increasing sales.

## Data Source:

Food Sales Predictions: https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view 

For this dataset, there were 8523 rows and 12 columns:

## Data Dictionary

<img width="337" alt="image" src="https://github.com/Souha-Kabtni/Sales_Predictions/assets/133057039/090a8f07-1815-4db7-8ea9-f1ebba64c5aa">

## To prepare this data, the data was cleaned, and the following processes were performed:

### Exploratory Data Analysis

    - Batrplots were visualized for each categorical column. 
    - Histograms were visualized for each numeric datatype column. 
    - This gave a good baseline for all of the categorical and numeric columns for univariate EDA.


### Explanatory Data Analysis

    - Three bar graphs were chosen and one line graph was chosen.
    - The bar graphs were chosen to show how the categories compare to each other. 
    - line graphs were chosen to show the trend of salaries over the past three years. 


### Explanatory Visuals



## Machine Learning Using the Following Models:

    - Linear Regression Model
    - Decision Tree Regressor Model
    - Tuned Decision Tree Regressor Model

## Models Evaluated & Results

+ Linear Regression Model (Testing Set):
  
    + R^2: 0.567 
    + RMSE: 1,092.858
 
+ Decision Tree Regressor Model (Testing Set):

    + R^2: 0.183 
    + RMSE: 1,501.460

+ Tuned Decision Tree Regressor Model (Testing Set):

    + R^2: 0.595 
    + RMSE: 1,057.443

The Final Model Chosen was a Regression Tree Model with the max_depth tuned to 5.

For the testing set on the model, 59.5 % of the variance in y was explained by x.

The Root Mean Squared Error had a calculation of $1,057.443.

Using this model to make sales predictions about food items sold at various stores would not be very reliable. !!!!!

## Recommendations


## Limitations & Next Steps

