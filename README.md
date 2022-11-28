
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

* Aplication of Trend
![image](https://user-images.githubusercontent.com/29828029/204370061-1d7fc491-39ca-4cdf-9094-84fe40db2181.png)


