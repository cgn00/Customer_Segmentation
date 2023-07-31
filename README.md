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

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) is an important step in any data analysis project. It involves the initial exploration and analysis of the data to identify patterns, trends, and relationships. EDA is often used to gain insights and to develop hypotheses about the data before applying more advanced statistical methods.

### Data Cleaning

Data cleaning is a crucial step in the exploratory data analysis process. It involves identifying and correcting errors, inconsistencies, and missing values in a dataset to ensure that it is accurate, complete, and usable for analysis. Data cleaning can involve tasks such as removing duplicates, filling missing values, correcting typos and formatting errors, and handling outliers. The goal of data cleaning is to ensure that the data is consistent and reliable, which is essential for making accurate inferences and drawing meaningful insights. By performing data cleaning, analysts can ensure that their analysis is based on high-quality data and that their conclusions are sound.

#### Removing duplicated data

It’s important to verify if there are duplicated data to remove them from the dataset, but as can be seen in the output there isn’t any data duplicated.

#### Filtering by Shipped Status

Filtering data is a common task in data analysis and can be useful to focus on specific subsets of the data. In this case, filtering by the ‘Shipped’ status can be useful to analyze only the orders that have been shipped, in order to do an accurate RFM analysis later.

### Data Visualization

Data visualization is an important tool for exploratory data analysis. It allows analysts to explore the data visually, identify patterns and trends, and communicate insights effectively. In this project, we used several Python libraries such as Seaborn, Matplotlib, and Plotly to create various types of visualizations, including scatter plots, bar charts, and heatmaps.

### RFM Analysis

RFM analysis is a customer segmentation technique that uses three variables to segment customers based on their buying behavior: recency, frequency, and monetary value. Recency refers to the time since a customer's last purchase, frequency refers to the number of purchases a customer has made, and monetary value refers to the total amount of money a customer has spent. In this project, we performed RFM analysis on the filtered sales data to segment customers into different groups based on their buying behavior.

## Clustering

Clustering is a common technique used in data analysis to group similar data points together. In this project, we used three clustering algorithms: KMeans, OPTICS, and DBSCAN to cluster customers based on their RFM scores. The resulting clusters can be useful for identifying different types of customers and developing targeted marketing strategies.

## Conclusion

Exploratory Data Analysis is a crucial step in any data analysis project. It involves data cleaning, data visualization, and data modeling techniques to gain insights and develop hypotheses about the data. In this project, we used various Python libraries and techniques to perform EDA on a sales dataset and used RFM analysis and clustering to segment customers based on their buying behavior. The resulting insights can be useful for developing targeted marketing strategies and improving customer engagement.
