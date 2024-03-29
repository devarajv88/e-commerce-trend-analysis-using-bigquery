
# E-commerce Trend Analysis


## Overview
This project focuses on analyzing the operations of a leading e-commerce retailer in Brazil. The dataset, comprising eight CSV files, provides a comprehensive view of 100,000 orders placed between 2016 and 2018. The analysis aims to extract valuable insights and offer actionable recommendations for the company.

## Table of Contents
1. [Problem Statement](#problem-statement)
2. [Dataset](#dataset)
3. [Dataset schema](#Dataset-schema)
4. [Tech Stack](#Tech-Stack)
5. [Data Exploration and Analysis](#Data-Exploration-and-Analysis)
6. [Actionable Insights & Recommendations](#actionable-insights--recommendations)

## Problem Statement

As a data analyst/scientist at the e-commerce retailer, the objective is to analyze the dataset and derive insights for the company. The analysis is structured into various sections, including initial exploration, in-depth exploration, evolution of e-commerce orders, impact on the economy, and analysis based on payments.

## Dataset

The dataset is available in the [Google Drive folder](https://drive.google.com/drive/folders/1TGEc66YKbD443nslRi1bWgVd238gJCnb). It consists of eight CSV files.

1. **customers.csv**: Information about customers, including IDs, unique IDs, zip codes, cities, and states.
2. **sellers.csv**: Details about sellers, such as IDs, zip codes, cities, and states.
3. **order_items.csv**: Data on orders, including order and item IDs, product IDs, seller IDs, and pricing details.
4. **geolocation.csv**: Geographical information with zip codes, latitude, longitude, cities, and states.
5. **payments.csv**: Payment-related data, including order IDs, payment sequences, types, installments, and values.
6. **orders.csv**: Order details, including order IDs, customer IDs, statuses, timestamps, and delivery information.
7. **reviews.csv**: Customer reviews with review IDs, order IDs, scores, titles, comments, and timestamps.
8. **products.csv**: Product information, including IDs, categories, name lengths, description lengths, photos, weights, lengths, heights, and widths.

The column description for these csv files is given below.

![1](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/a3261d6b-0f02-4f46-992b-90b9ceb33a13)

![2](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/09b2c04a-b849-486e-be54-4b30854969a0)

![3](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/8affcd08-decc-4645-8259-00c16a8c6e65)

![4](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/a2c6261e-ecd1-4b15-b69e-1733726464c3)

![5](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/0f1dfced-f72d-493b-b353-4abb0ee46bd2)

![6](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/ed8738bb-f921-40a0-8494-5ab6f38d671a)

![7](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/38a184fe-3406-4c99-ba0d-5c243e0e421c)

![8](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/014269a8-c02b-437f-853e-1279d63a23a0)

## Dataset schema
Dataset schema for the data provided above is shown below:

![schema](https://github.com/devarajv88/e-commerce-trend-analysis-using-bigquery/assets/63098473/73c0c8c7-57f0-480a-9cb2-8c187aa66e68)


## Tech Stack

- **SQL:** Used for querying the dataset and extracting relevant information.
- **Python:** Utilized for additional data analysis, visualization, and processing.
  - **Libraries**:
    - **Pandas**: Data manipulation and analysis.
    - **NumPy**: Numerical operations and array handling.
    - **Matplotlib**: Plotting visualizations.
    - **Seaborn**: Enhancing the aesthetics of visualizations.
## Data Exploration and Analysis

### a. Initial Exploration

#### SQL Query:
```sql
-- SQL query for delivery time analysis
SELECT order_id,
       order_delivered_customer_date - order_purchase_timestamp AS time_to_deliver,
       order_estimated_delivery_date - order_delivered_customer_date AS diff_estimated_delivery
FROM orders;
```
### b. In-depth Exploration

#### SQL Query:
```sql
-- SQL query for delivery time analysis
SELECT order_id,
       order_delivered_customer_date - order_purchase_timestamp AS time_to_deliver,
       order_estimated_delivery_date - order_delivered_customer_date AS diff_estimated_delivery
FROM orders;
```
### c. Evolution of E-commerce Orders in Brazil

#### SQL Query:
```sql
-- SQL query for delivery time analysis
SELECT order_id,
       order_delivered_customer_date - order_purchase_timestamp AS time_to_deliver,
       order_estimated_delivery_date - order_delivered_customer_date AS diff_estimated_delivery
FROM orders;
```
### d. Impact on Economy

#### SQL Query:
```sql
-- SQL query for delivery time analysis
SELECT order_id,
       order_delivered_customer_date - order_purchase_timestamp AS time_to_deliver,
       order_estimated_delivery_date - order_delivered_customer_date AS diff_estimated_delivery
FROM orders;
```
### e. Analysis on Sales, Freight and Delivery Time

#### SQL Query:
```sql
-- SQL query for delivery time analysis
SELECT order_id,
       order_delivered_customer_date - order_purchase_timestamp AS time_to_deliver,
       order_estimated_delivery_date - order_delivered_customer_date AS diff_estimated_delivery
FROM orders;
```


### f. Analysis Based on Payments

#### SQL Query:
```sql
-- SQL query for delivery time analysis
SELECT order_id,
       order_delivered_customer_date - order_purchase_timestamp AS time_to_deliver,
       order_estimated_delivery_date - order_delivered_customer_date AS diff_estimated_delivery
FROM orders;
```


## Actionable Insights & Recommendations

#### 1. Abcdef
- Step 1
- Step 2
#### 1. Abcdef
- Step 1
- Step 2
#### 1. Abcdef
- Step 1
- Step 2
#### 1. Abcdef
- Step 1
- Step 2
