# Task 1 (Level 1) - Exploratory Data Analysis
## Oasis Infobyte Data Analytics Internship

**Full Name:** Bakithi Gabashane  
**Track:** Data Analytics

## Project Overview

In this project, I performed Exploratory Data Analysis (EDA) on a customer shopping dataset from shopping malls in Istanbul. The aim was to explore customer purchasing behaviour, identify sales trends, compare product categories and evaluate shopping mall performance.

Using Python and data visualisation techniques, I examined the dataset to identify patterns and used the findings to suggest possible improvements to business performance.

## Dataset

**Source:** Kaggle - Customer Shopping Dataset  
**Original Dataset:** customer_shopping_data.csv  
**Dataset Shape:** 99,457 rows × 10 columns  
**Date Range:** 1 January 2021 - 8 March 2023

The dataset contains customer transaction records from different shopping malls in Istanbul. It includes information such as customer age, gender, product category, quantity purchased, price, payment method and shopping mall.

The initial inspection found no missing values.

## Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

## Analysis Performed

1. **Data Inspection:** Checked the dataset structure, data types, missing values and duplicate records.
2. **Descriptive Statistics:** Examined measures such as mean, median, mode and standard deviation to better understand the numerical data.
3. **Sales Trends:** Analysed monthly and quarterly sales to identify changes in revenue over time.
4. **Customer Demographics:** Explored purchasing patterns across different genders and age groups.
5. **Product Performance:** Compared total revenue, quantities sold and average transaction values across product categories.
6. **Payment Methods:** Analysed the distribution of transactions and revenue across different payment methods.
7. **Correlation Analysis:** Used a correlation heatmap to examine relationships between numerical variables.
8. **Shopping Mall Performance:** Compared total sales, transaction counts and average transaction values across shopping malls.

## Key Findings

| Finding | Result |
|---|---|
| Total Revenue | 251,505,794.25 |
| Total Transactions | 99,457 |
| Average Transaction Value | 2,528.79 |
| Highest Revenue Category | Clothing (94.7 million) |
| Highest Average Transaction Value | Technology (11,582) |
| Top Performing Mall | Mall of Istanbul |
| Majority of Customers | Female (59.8%) |
| Highest Revenue Age Group | 35–44 |
| Most Used Payment Method | Cash (44.6%) |

## Business Recommendations

Based on the findings from the analysis, the following recommendations could help improve sales performance and customer engagement.

1. **Focus on Clothing and Technology:** Clothing generates the highest revenue, while Technology has the highest average transaction value. Maintaining sufficient clothing stock and promoting technology products could help support sales growth.

2. **Improve Customer Segmentation:** Although customers aged 35–44 generate the highest total revenue, age shows little correlation with spending behaviour. The business could focus more on purchasing habits, product preferences and spending patterns when developing marketing campaigns.

3. **Prioritise High-Performing Malls:** Mall of Istanbul and Kanyon record the highest sales and transaction volumes. These locations could be prioritised for promotional campaigns and popular product ranges, while lower-performing malls could benefit from strategies aimed at increasing transactions.

4. **Encourage Digital Payments:** Cash accounts for the largest share of transactions. Offering incentives such as loyalty points or discounts for card payments could encourage digital payment adoption and potentially reduce cash handling costs.

5. **Explore Male Customer Engagement:** Female customers account for a larger share of transactions and revenue. The business could investigate whether its current product range meets the needs of male customers and explore opportunities to attract a wider customer base.

## Files in This Repository

| File | Description |
|---|---|
| `EDA_Customer_Shopping.ipynb` | Jupyter Notebook containing the analysis and visualisations |
| `customer_shopping_data.csv` | Original dataset used for the analysis |
| `README.md` | Project overview, findings and recommendations |

## Conclusion

This project helped me gain practical experience in exploring datasets, identifying patterns and presenting findings through data visualisation. It also allowed me to practise using Python libraries such as Pandas, Matplotlib and Seaborn to turn raw data into useful insights.

The analysis highlighted differences in product performance, customer purchasing behaviour and shopping mall sales, showing how exploratory data analysis can support business decisions.