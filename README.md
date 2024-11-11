
# E-commerce Data Analysis with Python and SQL

This project analyzes e-commerce data using Python and SQL to extract meaningful insights by answering different business questions. The results of all the SQL queries that are mentioned in the Jupyter notebook are also cross-verified in the MySQL Workbench.

# Prerequisites
- Python
- Jupyter Notebook
- MySQL database

# Data Source
The data used in this project is sourced from the Target dataset available on Kaggle:
https://www.kaggle.com/datasets/devarajv88/target-dataset?select=products.csv

Download the data consisting of seven files and save them to a local folder. The path to the files can be used in the code, please make sure you change it to match your local path.

# Setup

To run this project, you need to have the following libraries installed:
- import numpy as np
- import pandas as pd
- import mysql.connector
- import os
- import matplotlib.pyplot as plt
- import seaborn as sns

Also please make sure you have a MySQL database set up and the necessary credentials to connect to it.

# Database connection
To connect to the MySQL database, update the following code with your database credentials:
db_con = mysql.connector.connect(
    host='Host name',
    user='username',
    password='your password',
    database='your target database name'
)

Change the username, password, host, port number and database name according to your own credentials.

# Usage
 1. Download the dataset from the above given link and save it to a local folder
 2. ####  Data Ingestion:
The project includes a data ingestion process that automates the creation of tables and insertion of data from CSV files into the MySQL database. The process handles data type conversions and NULL values.
 - Make changes to the data ingestion code based on your database credentials, dataset path and file names etc.
 - This will take time to run due to the large amount of data in multiple tables. Once the data has been successfully inserted, you can comment out the code as it is no longer needed. You just need to follow the steps mentioned in Jupyter notebook and can start analysing the data.

# Analysis
The project includes various analyses, such as:
- Listing unique customer cities
- Counting orders placed in 2017
- Calculating total sales per product category
- Analyzing payment installments
- Visualizing customer distribution by state
- Examining order trends by month
- Calculating average products per order by city
- Analyzing revenue contribution by product category
- Investigating correlation between product price and number of times a product has been purchased
- Ranking sellers by revenue
- Calculating cumulative sales per month
- Computing year-over-year growth rate of total sales
Each analysis is accompanied by SQL queries and, where applicable, visualizations using matplotlib and seaborn.

# Project Structure
- eCommerce-sql-python.ipynb: Main script containing the python code and SQL queries
- README.md: This file which contain all necessary info about the project

