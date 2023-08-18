![image](https://github.com/Souha-Kabtni/Sales_Predictions/assets/133057039/b3660500-4692-4874-a7ad-d5a5c706dbf1)

# Increasing Food Sales Predictions

Souha Kabtni

## Analyzing Products & Outlets properties in increasing sales

A sales prediction for food items sold at various stores. The goal of this is to help the retailer understand the properties of products and outlets that play crucial roles in increasing sales.

## Data Source:

Click [ here ](https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view) to download the dataset.

For this dataset, there were ``` 8523 rows```  and ``` 12 columns```.

## Data Dictionary

![image](https://github.com/Souha-Kabtni/Sales_Predictions/assets/133057039/22a160da-98dd-4c44-bdbe-64d5aea3ecd1)

## To prepare this data, the data was cleaned, and the following processes were performed:

### Exploratory Data Analysis

    - Batrplots were visualized for each categorical column. 
    - Histograms were visualized for each numeric datatype column. 
    - This gave a good baseline for all of the categorical and numeric columns for univariate EDA.

![image](https://github.com/Souha-Kabtni/Sales_Predictions/assets/133057039/d6aa2b52-a48b-4fb8-94d3-210a9c6c3472)

This histogram shows that the majority of the Item Outlet Sales are around $2000,000.

### Explanatory Data Analysis

    - 1 barplot and one heatmap were chosen.
    - The barplot was chosen to show how the category compare to each other. 
    - The heatmap was chosen to show which numerical variable most correlates with our target variable. 

### Explanatory Visuals

<img width="653" alt="image" src="https://github.com/Souha-Kabtni/Sales_Predictions/assets/133057039/3baf98c5-865b-43cc-b0a6-955b415d9112">

Item visibility over item type by item fat content demonstrates that Seafood with regular fat is the most visible item while Breakfast has the highest visibility in terms of low fat.

<img width="376" alt="image" src="https://github.com/Souha-Kabtni/Sales_Predictions/assets/133057039/769b8008-cff1-4d88-8c01-b24ce7491497">

+ With a positive correlation of ``` 0.57``` , Item_MRP and Item_Outlet_Sales moderately correlate.
+ With a negative correlation of ``` -0.13```  and ``` -0.049```  between Item_Visibility and Outlet_Establishment_Year respectively with Item_Outlet_Sales.
+ Conclusion: The more the product is high in price, the more it is sold.

## Machine Learning Using the Following Models:

    - Linear Regression Model
    - Decision Tree Regressor Model
    - Tuned Decision Tree Regressor Model

## Models Evaluated & Results

+ Linear Regression Model (Testing Set):
  
    + R^2: ``` 0.567 ``` 
    + RMSE: ```  1,092.858 ``` 
 
+ Decision Tree Regressor Model (Testing Set):

    + R^2:```  0.183 ``` 
    + RMSE:```  1,501.460 ``` 

+ Tuned Decision Tree Regressor Model (Testing Set):

    + R^2: ``` 0.596 ``` 
    + RMSE:```  1,055.975``` 

The Final Model Chosen was a Regression Tree Model with the max_depth, min_samples_split, and min_samples_leaf tuned to ``` 5``` , ``` 6``` , and ``` 15``` , respectively.

For the testing set on the model, ``` 59.6 %```  of the variance in y was explained by x.

The Root Mean Squared Error had a calculation of ``` $1,055.975``` .

Using this model to make sales predictions about food items sold at various stores would not be very reliable. A prediction error of ``` $1,055.975```  (that represents almost 52.8% of the mean values of the Item-Outlet sales) cannot be overlooked.

## Recommendations

Given that the results of the tuned Decision Tree Regressor Model did not yield reliable results, I recommend the following:
+ Dedicate more time in the feature engineering phase so as to select and transform the most relevant variables from raw data when creating a predictive model using machine learning;
+ The use of alternative models and the adjusting of their hyperparameters (examples might be the Random Forest Model).

## Limitations & Next Steps

The generated "poorly performant" model might be emanating from these 2 reasons:
+ The predefined features might have not been directly impacting our target variables of item_outlet_sales;
+ Feature engineering was not given the utmost importance since all found features were selected to help in the prediction of the model.

## For Further Information
For any additional questions, please contact:

Souha Kabtni
souha.kabtni.data@gmail.com
