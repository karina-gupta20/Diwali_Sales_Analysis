Sure, here's a concise version of the README file:

---

# Diwali Sales Analysis

## Project Overview
This project analyzes Diwali sales data to gain insights into customer demographics, purchasing behaviors, and sales trends.

## Dataset
The dataset contains sales data with 11,251 rows and 15 columns, including attributes like User_ID, Gender, Age Group, Marital_Status, State, Occupation, Product_Category, Orders, and Amount.

## Installation
Install the required libraries using:
```bash
pip install numpy pandas matplotlib seaborn
```

## Data Preprocessing
1. **Load Data:** 
   ```python
   df = pd.read_csv('diwali Sales Data.csv', encoding='unicode_escape')
   ```
2. **Inspect and Clean Data:** Check for null values and drop them.
   ```python
   df.dropna(inplace=True)
   ```
3. **Convert Data Types:** Convert `Amount` to integer.
   ```python
   df['Amount'] = df['Amount'].astype('int')
   ```

## Exploratory Data Analysis
- **Gender Analysis:** Count and total purchase amount by gender.
- **Age Group Analysis:** Count and total purchase amount by age group.
- **State-wise Analysis:** Orders and sales amount from top 10 states.
- **Marital Status Analysis:** Count and total purchase amount by marital status.
- **Occupation Analysis:** Count and total purchase amount by occupation.
- **Product Category Analysis:** Count and total purchase amount by product category.
- **Top Sold Products:** Most sold products by number of orders.

## Conclusion
The primary buyers are married women aged 26-35 years from Uttar Pradesh, Maharashtra, and Karnataka, working in IT, Healthcare, and Aviation, predominantly purchasing Food, Clothing, and Electronics.
