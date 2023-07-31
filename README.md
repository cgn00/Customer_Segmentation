# Customer_Segmentation
 This is a customer segmentation problem to problem to participate in the natasquad competition

This project provides instructions and code for analyzing sales data. The goal is to perform exploratory data analysis (EDA) to identify patterns and trends in the data and to develop insights for decision-making.

## Prerequisites

To run this code, you will need to have the following Python packages installed:

- pandas
- numpy
- seaborn
- matplotlib
- plotly
- datetime
- sklearn

You can install these packages using pip by running the following command:

```
pip install pandas numpy seaborn matplotlib plotly scikit-learn
```

## Importing Necessary Packages

This section imports the necessary Python packages for data manipulation, visualization, and machine learning. The packages used are:

- os
- pandas
- numpy
- seaborn
- matplotlib
- plotly
- datetime
- StandardScaler from sklearn.preprocessing
- KMeans, OPTICS, DBSCAN from sklearn.cluster
- NearestNeighbors from sklearn.neighbors
- make_subplots from plotly.subplots

## Loading the Data

The sales data is loaded from a CSV file using the pandas `read_csv()` function. The data is then cleaned by converting the 'ORDERDATE' column to a datetime format and filtering the sales data to only include rows where the 'STATUS' column is 'Shipped'. The resulting DataFrame includes columns for order number, quantity ordered, price each, order line number, sales, order date, order status, quarter ID, month ID, year ID, product line, MSRP, product code, customer name, phone number, address line 1 and 2, city, state, postal code, country, territory, contact last name, contact first name, and deal size.

## Exploratory Data Analysis (EDA)

This section covers data cleaning and filtering the data by shipped status. Data cleaning involves identifying and correcting errors, inconsistencies, and missing values in the dataset to ensure that it is accurate, complete, and usable for analysis. Filtering by shipped status is useful to analyze only the orders that have been shipped, in order to do an accurate RFM analysis later.

## Conclusion

This project provides a starting point for analyzing sales data. With the code provided, you can perform EDA and gain insights into the data to make informed decisions. By using the appropriate Python packages, you can manipulate and visualize the data, and apply machine learning techniques such as clustering to gain further insights.