# Timeseries Forecasting and Sales Analysis

## Table of Contents
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Data Overview](#data-overview)
- [Marketing Analysis](#marketing-analysis)
- [Operational Analysis](#operational-analysis)
- [Retail Product Analysis](#retail-product-analysis)
- [Customer Relationship Management](#customer-relationship-management)
- [Results](#results)
- [Conclusion](#conclusion)
- [How to Run the Project](#how-to-run-the-project)
- [Project Structure](#project-structure)
- [Acknowledgements](#acknowledgements)

## Introduction
This project aims to provide valuable insights from customer transaction data over a one-year period. The goal is to derive strategies that address key questions for various departments within the organization, including Marketing, Operations, Retail Products, and Customer Relationship Management.

## Project Overview
The analysis encompasses customer segmentation, sales forecasting, and identifying high-value products and customers. By leveraging machine learning models and time series forecasting techniques, the project aims to enhance customer segmentation, forecast sales accurately, improve product placement, and reduce customer churn.

## Data Overview
The dataset includes 525,461 rows and 8 columns, representing one year of transactions. Key features include:
- `Invoice`: Unique identifier for each transaction.
- `StockCode`: Unique identifier for each product.
- `Description`: Product name.
- `Quantity`: Quantity of products per transaction.
- `InvoiceDate`: Date and time of the transaction.
- `Price`: Price per unit.
- `Customer ID`: Unique identifier for each customer.
- `Country`: Customer's country of residence.

## Marketing Analysis
### Customer Clustering and RFM Analysis
- **Model**: K-Means Clustering using Recency, Frequency, and Monetary (RFM) metrics.
- **Recency**: Days since the last purchase.
- **Frequency**: Total number of purchases.
- **Monetary**: Total amount spent by the customer.

#### Clusters:
1. **Recent Buyer**: Recency score 0-50.
2. **Potential Buyer**: Recency score 50-150.
3. **Occasional Buyer**: Recency score 150-250.
4. **Long Time Ago**: Recency score 250-350.

## Operational Analysis
### Sales Forecasting
- **Model**: SARIMA (Seasonal Autoregressive Integrated Moving Average)
- **Purpose**: Forecast sales at the country level for the next quarter.

#### Key Insights:
1. Focus on G7 countries and regions with high NRI presence.
2. Develop operations strategy based on historical sales data.

## Retail Product Analysis
### Daily Sales Forecasting
- **Model**: Prophet library for time series forecasting.

### Market Basket Analysis
- **Model**: Apriori algorithm to identify product co-purchase patterns.

#### Key Insights:
1. Upsell top 20 purchasing products.
2. Utilize ABI index heatmap for cross-selling opportunities.

## Customer Relationship Management
### Churn Detection
- **Model**: Random Forest Classifier
- **Purpose**: Predict customer churn at the country and month levels.

#### Key Insights:
1. Focus on reducing churn in high churn rate countries.
2. Tailor strategies for different customer segments.

## Results
The analysis provided actionable insights for different departments, enhancing customer segmentation, improving sales forecasting, and identifying key strategies for marketing, operations, and product placement.

## Conclusion
By leveraging machine learning models and time series forecasting, the project successfully addressed key business questions and provided data-driven strategies to improve customer segmentation, forecast sales, and reduce customer churn.

## How to Run the Project
1. Run the Jupyter notebook: `jupyter notebook Timeseries_Forecasting_project.ipynb`

## Project Structure
- `Timeseries_Forecasting_project.ipynb`: Jupyter notebook with the complete analysis.
- `Fittlyf_Sales_Analysis.pdf`: Detailed report of the sales analysis.


