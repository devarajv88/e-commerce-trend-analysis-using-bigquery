
# E-commerce Trend Analysis


## Overview
This project focuses on analyzing the operations of a leading e-commerce retailer (Target) in Brazil. The dataset, comprising eight CSV files, provides a comprehensive view of 100,000 orders placed between 2016 and 2018. The analysis aims to extract valuable insights and offer actionable recommendations for the company.

## Table of Contents
1. [Problem Statement](#problem-statement)
2. [Key Analytical Inquiries](#key-analytical-inquiries)
3. [Dataset](#dataset)
4. [Dataset schema](#dataset-schema)
5. [Tech Stack](#tech-stack)

## Problem Statement

As a data analyst/scientist at the e-commerce retailer, the objective is to analyze the dataset and derive insights for the company. The analysis is structured into various sections, including initial exploration, in-depth exploration, evolution of e-commerce orders, impact on the economy, and analysis based on payments.

## Key Analytical Inquiries
Through a series of insightful questions, we navigate the dataset's depths, driven by curiosity and the quest for knowledge.

1. Check the structure & characteristics of the dataset:

    a. Data type of all columns in the "customers" table.
    
    b. Get the time range between which the orders were placed.

    c. Count the Cities & States of customers who ordered during the given period.

2. In-depth Exploration:

    a. Is there a growing trend in the no. of orders placed over the past years?

    b. Can we see some kind of monthly seasonality in terms of the no. of orders being placed?

    c. During what time of the day, do the Brazilian customers mostly place their orders? (Dawn, Morning, Afternoon or Night)

        i. 0-6 hrs : Dawn
        
        ii. 7-12 hrs : Mornings
        
        iii. 13-18 hrs : Afternoon
        
        iv. 19-23 hrs : Night

3. Evolution of E-commerce orders in the Brazil region:

    i. Get the month on month no. of orders placed in each state.

    ii. How are the customers distributed across all the states?

4. Impact on Economy: Analyze the money movement by e-commerce by looking at order prices, freight and others.

    i. Get the % increase in the cost of orders from year 2017 to 2018 (include months between Jan to Aug only). We can use the "payment_value" column in the payments table to get the cost of orders.

    ii. Calculate the Total & Average value of order price for each state.

    iii. Calculate the Total & Average value of order freight for each state.

5. Analysis based on sales, freight and delivery time.

    i. Find the no. of days taken to deliver each order from the order’s purchase date as delivery time. Also, calculate the difference (in days) between the estimated & actual delivery date of an order. Do this in a single query.

       We can calculate the delivery time and the difference between the estimated & actual delivery date using the given formula:

        * time_to_deliver = order_delivered_customer_date - order_purchase_timestamp

        * diff_estimated_delivery = order_delivered_customer_date - order_estimated_delivery_date

    ii. Find out the top 5 states with the highest & lowest average freight value.

    iii. Find out the top 5 states with the highest & lowest average delivery time.

    iv. Find out the top 5 states where the order delivery is really fast as compared to the estimated date of delivery.

    We can use the difference between the averages of actual & estimated delivery date to figure out how fast the delivery was for each state.

6. Analysis based on the payments:

    i. Find the month on month no. of orders placed using different payment types.

    ii. Find the no. of orders placed on the basis of the payment installments that have been paid.



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

## Dataset schema
Dataset schema for the data provided above can be acced from [**here**](https://drive.google.com/file/d/1fMIzsB2AN5Cwu8EUt8bU3LYUc6w3NCI-/view?usp=drive_link)

## Tech Stack

- **SQL:** Used for querying the dataset and extracting relevant information.
- **Tableau:** Utilized for additional data analysis and visualization.
