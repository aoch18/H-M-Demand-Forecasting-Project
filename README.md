
## H&M Demand Forecasting Project
Application of Time Series to predict H&M Demand

## Datasource
Initials CSV Files
* articles.csv
* customers.csv
* transactions_train

https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data

## Import Data from Python to MySQL

![image](https://user-images.githubusercontent.com/29828029/204364486-7212c646-ea18-43de-b3fa-6be9b3a9346f.png)

we split the orders table into 3 parts due to the large number of records (more 30 millions of rows)

## Creating the table Order Category

![image](https://user-images.githubusercontent.com/29828029/204366684-92254d3c-2916-4897-b696-f85e794b79b0.png)

We create the table Order Category to determine the sales by category.

## Creating CSV to Predict Model
Now we create a new file named orders_category.csv

## Initials Step to create Predict Model

* We Import file csv to a new Notebook file named TimeSeriesModel.py
* Now we determine best selling category into sales channel 1

![image](https://user-images.githubusercontent.com/29828029/204366832-c057e995-adf5-4887-90bd-fb63d5b837ba.png)

## Creating table to Time Series Model

* We going to determine demand from 'Garment Upper body' category

![image](https://user-images.githubusercontent.com/29828029/204369249-df54eaa6-ef1e-432b-a68a-ec567212b3ab.png)

* Historic Demand
![image](https://user-images.githubusercontent.com/29828029/204369349-70742c9a-9757-4c08-8ca4-7dd2b54e8870.png)

## Trend Component

* Creating t_dias column

![image](https://user-images.githubusercontent.com/29828029/204369723-e2826120-a610-434c-931d-21c16a1d72a8.png)

* Application of Trend
![image](https://user-images.githubusercontent.com/29828029/204370061-1d7fc491-39ca-4cdf-9094-84fe40db2181.png)

## Cycle Component

### Polynomial Trend
* Creating Polynomials columns

![image](https://user-images.githubusercontent.com/29828029/204370852-555786ac-771c-4c71-98d0-9a5ef61ff0da.png)

* Application of polynomial to the square

![image](https://user-images.githubusercontent.com/29828029/204370947-99210f9c-c169-4a01-b0e0-24829250f0f0.png)

### B-Splines
* Creating B-Splines columns

![image](https://user-images.githubusercontent.com/29828029/204371536-d3734d37-0d75-4642-9f92-472868b2c75b.png)

* Application of B-Splines

![image](https://user-images.githubusercontent.com/29828029/204372090-c4bfe2b4-23ac-4674-b5b6-c71c21eef499.png)

## Season Component 

* Creating categoricals columns of day and month

![image](https://user-images.githubusercontent.com/29828029/204372336-7164565c-f28a-4613-8335-61109fe9e0ca.png)

* Creating dummys columns 

![image](https://user-images.githubusercontent.com/29828029/204372472-6eebf9b9-bfde-445b-a973-88956cf16c2a.png)

* Application of Season Component

![image](https://user-images.githubusercontent.com/29828029/204372653-7e76ccbb-8043-4e17-a2bb-177e5fc967a5.png)

## Final Model

* To apply final model to need normalized the columns from others components

![image](https://user-images.githubusercontent.com/29828029/204373204-e0d4650b-1ec5-41de-b408-7a1b2513a1a5.png)

* Application of Final Model

![image](https://user-images.githubusercontent.com/29828029/204373327-a160cff3-4d72-433c-88c8-ff35b5252ec7.png)

## Validating of Results

* Validation of error to every model

![image](https://user-images.githubusercontent.com/29828029/204373594-2162bfac-5634-4a2d-b96e-af6de69ca476.png)

* Validation into test period 

![image](https://user-images.githubusercontent.com/29828029/204373693-50201e37-7fed-4da3-8b9f-9a1c4e4b2c79.png)

![image](https://user-images.githubusercontent.com/29828029/204373746-ae031dee-8fa5-4828-8179-309f2000ac2d.png)

## Conclusion

We concluded that best model to case is season model, due to Final model have over feature





