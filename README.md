# Instacart Customer Behavior Analysis
![Instacart](instacart.png)

## Project Overview
This project involves exploring and analyzing a dataset from Instacart, a popular grocery delivery platform. The dataset was released as part of a Kaggle competition in 2017 and has been modified for this project. The goal is to gain insights into the shopping habits of Instacart customers by performing data cleaning, preprocessing, and exploratory data analysis (EDA).

## Table of Contents

1. Project Description
2. Data
3. Project Structure
4. Methodology
- Data Overview
- Data Preprocessing
- Data Analysis
5. Conclusion
6. Future Work

## Project Description
In this project, we work with data from Instacart, a grocery delivery platform where customers can place orders to be delivered directly to them. The dataset used in this project has been modified from its original version to include missing and duplicate values and reduce its size for faster calculations.

Our goal is to clean the data and generate insights into the shopping patterns of Instacart customers. We will explore various aspects of customer behavior, such as the timing of orders, reorder habits, and popular products.

## Data
The dataset consists of five CSV files, each representing a different aspect of the Instacart data:

instacart_orders.csv: Contains information about individual orders.

-  order_id: Unique identifier for each order.
- user_id: Unique identifier for each customer.
- order_number: Number of times this customer has placed an order.
- order_dow: Day of the week the order was placed.
- order_hour_of_day: Hour of the day the order was placed.
- days_since_prior_order: Number of days since the customer's last order.


products.csv: Contains information about the products available on Instacart.

- product_id: Unique identifier for each product.
- product_name: Name of the product.
- aisle_id: Identifier for the grocery aisle.
- department_id: Identifier for the grocery department.


order_products.csv: Contains information about the products in each order.

- order_id: Unique identifier for each order.
- product_id: Unique identifier for each product.
- add_to_cart_order: Order in which the items were added to the cart.
- reordered: Indicates if the product has been ordered before (1) or not (0).


aisles.csv: Contains information about the grocery aisles.

- aisle_id: Unique identifier for each aisle.
- aisle: Name of the aisle.


departments.csv: Contains information about the grocery departments.

- department_id: Unique identifier for each department.
- department: Name of the department.



## Project Structure
This project is structured into three main steps:

1. Data Overview: Review the contents and structure of the data files.
2. Data Preprocessing: Clean and prepare the data for analysis.
3. Data Analysis: Perform exploratory data analysis (EDA) to uncover patterns and insights.

## Methodology
1. Data Overview
The project begins with an overview of the data, where we load each of the five CSV files and inspect their contents. Given the nonstandard formatting, we adjust parameters in pd.read_csv() to properly load the data.
2. Data Preprocessing
Data preprocessing involves several key steps:

- Data Type Verification: Ensure ID columns are integers and other columns have appropriate data types.
- Missing Values: Identify and handle missing values appropriately, either by filling them in or dropping the rows.
- Duplicate Values: Detect and remove duplicate entries from the dataset to ensure accuracy.

3. Data Analysis
The analysis is divided into three parts:
Part A (Mandatory)

- Verify that values in order_hour_of_day (0-23) and order_dow (0-6) are sensible.
- Create a plot showing the distribution of orders by hour of the day.
- Create a plot showing the distribution of orders by day of the week.
- Analyze how long customers wait before placing their next order, identifying the minimum and maximum values.

Part B (Mandatory)

- Compare the distribution of order times on Wednesdays and Saturdays using histograms.
- Explore the distribution of how frequently customers place orders.
- Identify the top 20 most frequently ordered products.

Part C (Optional - Complete at least 2)

- Analyze the typical number of items customers buy in a single order.
- Identify the top 20 most frequently reordered products.
- Calculate the proportion of orders that are reorders for each product.
- Determine the proportion of reordered items for each customer.
- Identify the top 20 products most frequently added to the cart first.

## Conclusion
This analysis provides valuable insights into the shopping behavior of Instacart customers. The findings reveal patterns in order timing, customer preferences for certain products, and reorder habits. These insights can help Instacart optimize its services and improve the customer experience.

## Future Work
Future analysis could include:

- Segmenting customers based on their shopping habits and preferences.
- Applying machine learning models to predict future orders or recommend products to customers.
- Exploring the relationship between product categories and reorder frequency.
