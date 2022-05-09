# ClassProjectETL

## Project Authors

Christian Adiputra: matplotlib, top 10 and botton 10 country data\
David Cheung: jupyter notebook and SQL connection\
Maica Tran: SQL processing\
Vik Shah: clean and extract data\
Vasu Vinjirapu: obeserve the transformation and data-loading process. 

## Project Contents
1. Project Parts & Charter
2. Project Applications
3. Project Introduction & Background
4. Project Report
   * Extract
   * Transform
   * Load
5. Project Insights & Conclusion

## 1. Project Parts & Charter

(1) Resources/ 2015-2022.csv "World Happiness Report"\
(2) Resources/ Cost of Living Index.csv

## 2. Project Applications

Pandas\
Matplotlib\
Sqlalchemy\
Postgresql



## 3. Project Introduction & Background

Extract world happiness index from kaggle.com data source\
Transform the data files (.csv) into dataframes and cleanse\
Load dataframes into tables or "datawarehouse" e.g. PostgreSQL

## 4. Project Report

### (i). Extract

3 CSV files were extracted from https://www.kaggle.com/. The datasets consist of two type of data: happiness index (2020 and 2021) and cost-of-living index.

### (ii). Transform

The tranformation process started by forming dataframes for each CSV file. Column names were modified to align with the database tables. Aggregation were done between happiness index 2020 and 2021 to produce average index between the two years for each country.

### (iii). Load

Database were set within Postgrestsql, consisting 3 tables to represent each dataframe. Using SQLAlchemy, a connection was established between Python and PostgresSQL. Data was loaded, and tested to confirm the connection.

## 5. Project Insights & Conclusion

The datasets were chosen to identify correlations between countries' happiness index and their cost-of-living. The finding suggests that higher cost-of-living is not negatively correlated to the countries' happiness. This is shown as most countries in the top 10 happiest list are also within the top 10 of highest cost-of-living index.

