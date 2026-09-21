# Online Retail Sales Forecasting and Customer Insights System

## Project Overview

This project analyzes online retail transaction data to identify sales trends, customer behavior, product performance, and business insights.

The project includes:

- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- KPI and Statistical Analysis
- RFM Customer Segmentation
- Feature Engineering
- Machine Learning-based Sales Forecasting
- Future Sales Prediction
- Business Insights and Recommendations

## Dataset

The project uses the Online Retail Dataset containing transaction-level retail data.

**Original Dataset:** 541,909 rows × 8 columns

**Final Dataset:** 524,878 rows × 11 columns

**Data Period:** December 1, 2010 – December 9, 2011

## Data Preprocessing

The following steps were performed:

- Removed duplicate records
- Removed invalid quantities and prices
- Removed cancelled transactions
- Converted transaction dates into datetime format
- Created `TotalSales = Quantity × UnitPrice`
- Created Year and Month features

## Exploratory Data Analysis

The analysis covers:

- Monthly sales trends
- Top products by revenue and quantity
- Revenue by country
- Customer purchasing behavior
- Important business KPIs

### Key KPIs

- Total Revenue: £10,642,110.80
- Total Orders: 19,960
- Unique Customers: 4,338
- Unique Products: 3,922
- Average Order Value: £533.17

## Customer Analysis

RFM (Recency, Frequency, Monetary) analysis was used to segment customers.

| Segment | Customers |
|---|---:|
| Champions | 1,267 |
| Potential/Loyal | 1,276 |
| At Risk | 989 |
| Inactive | 806 |

## Sales Forecasting

Daily sales were converted into a calendar-based time series.

Features included:

- Calendar features
- Lag features
- Rolling averages
- Weekly sales patterns

Three machine learning models were evaluated:

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 25,273.72 | 34,520.07 | -0.2196 |
| Gradient Boosting | 14,139.41 | 24,857.35 | 0.3676 |
| Random Forest | 13,117.32 | 23,491.33 | 0.4352 |

The Random Forest model was used for the seven-day future sales forecast.

## Future Forecast

The model predicted approximately **£309,214.22** in total sales for the seven-day forecast period.

## Business Insights

- Sales showed clear weekly and monthly patterns.
- A small group of customers contributed significant revenue.
- RFM analysis identified different customer engagement groups.
- Historical sales patterns can support demand and inventory planning.
- Customer segmentation can support targeted retention strategies.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Project Files

- `Online_Retail_Sales_Forecasting.ipynb` – Complete analysis and machine learning notebook
- `Online_Retail_Sales_Forecasting_Report.pdf` – Project report
- `data.csv` – Dataset

## Author

**Lavanya R**
