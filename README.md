# Task 3 (Level 1) - Data Cleaning
## Oasis Infobyte Data Analytics Internship

Full Name: Bakithi Gabashane
Track: Data Analytics

## Project Overview

In this project, I cleaned the Titanic dataset and prepared it for analysis. 
The notebook walks through each step, from identifying data quality issues to choosing how to handle them, with an explanation for each decision.

## Dataset

Source: Titanic Dataset 
Original dataset: titanic.csv
Original dataset shape: 418 rows x 12 columns

Cleaned dataset: titanic_cleaned.csv
Cleaned dataset shape: 418 rows x 11 columns

## Tools and Libraries used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

## Problems found in the raw data:

|Issue|Column|Detail|
|---|---|---|
| Missing values | Age | 86 missing values (20.6%)|
| Missing values | Fare | 1 missing value (0.2%) |
| Missing values | Cabin | 327 missing values (78.2%) |
| Inconsistent formatting | Sex | Lowercase (male/female)|
| Wrong data type | PassengerId | Integer instead of string |
| Wrong data type | Survived | Integer instead of category |
| Wrong data type | Pclass | Integer instead of category |
| Outliers | Age | Values beyond IQR bounds |
| Outliers | Fare | Values beyond IQR bounds |

## Cleaning Steps Performed

1. Checked for duplicates and none were found.
2. Dropped Cabin column: 78.2% of values were missing which is too many to impute meaningfully.
3. Imputed Age column: filled 86 missing values with median age 27.0.
4. Imputed Fare column: filled 1 missing value with median fare 14.45.
5. Standardised Sex column: capatilised values in the Sex column using str.capitalize().
6. Fixed data types: PassengerId to string, Survived and Pclass to category.
7. Outlier detection: used IQR method on Age (36 outliers) and Fare (55 outliers). 
8. Outlier handling: capped outliers at IQR bounds to preserve all rows while limiting extreme values. 

- Age values capped to range [3.88, 54.88]
- Fare values above 66.84 were capped.

## Before vs After Summary

| Metric | Before | After |
| --- | --- | --- |
| Rows | 418 | 418 |
| Columns | 12 | 11 |
| Missing values | 414 | 0 |
| Duplicated rows | 0 | 0 |
| Age missing | 86 | 0 |
| Fare missing | 1 | 0 |
| Cabin | 327 missing | Dropped |
| Sex formatting | lowercase | Capitalized |
| Outliers | Present | Capped |

## Files in the Repository

| File | Description |
| --- | --- |
| `Data_Cleaning_Titanic.ipynb` | Jupyter Notebook with full cleaning workflow |
| `titanic.csv` | Original raw dataset |
| `titanic_cleaned.csv` | Final cleaned dataset |
| `README.md` | Project documentation |

## Key Decisions and Justifications

**Why missing values in Age and Fare columns with the median?**  
The mean is sensitive to extreme outliers (values outside the IQR bounds), however the median gives a more reliable estimate of a typical passenger’s age and fare.

**Why remove the Cabin column?**
About 78.2% of values are missing in the Cabin column. 
Filling in that many gaps would mean making too many assumptions, so I removed the column.

**Why cap outliers instead of removing rows?**  
The outliers may represent real passengers. 
Capping them keeps those records in the dataset while reducing the effect of extreme values on later analysis.

