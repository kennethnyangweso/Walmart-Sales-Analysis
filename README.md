# 📊 Walmart Sales Exploratory Data Analysis (EDA)
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-orange?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green?logo=plotly)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-teal)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-red?logo=jupyter)


This project performs an in-depth **Exploratory Data Analysis (EDA)** on Walmart sales data to uncover meaningful business insights, identify patterns, and understand key factors influencing store performance.

---

## 🧠 Project Overview

Retail companies depend on analytics to understand customer behavior, optimize inventory, and maximize revenue.  
This project focuses on **data understanding and insight generation**, not machine learning modeling.

### Objectives:
- Analyze overall Walmart sales trends
- Identify seasonal & time-based sales behavior
- Compare performance across stores
- Assess the effect of holidays on sales
- Present insights through clear visualizations

---

## 📁 Repository Structure

| File / Folder | Description |
|--------------|------------|
| `Walmart Notebook.ipynb` | Main notebook containing all analysis & visualizations |
| `walmart.csv` | Original dataset |
| `Walmart_sales_analysis.csv` | Cleaned / processed dataset |
| `README.md` | Project documentation |
| `LICENSE` | License file 

## ✔️ Steps Performed

- Data cleaning & formatting

- Handling missing values 

- Time-series exploration

- Store-wise sales comparison

- Seasonal pattern exploration

- Statistical summaries

## 📈 Exploratory Data Analysis

## Univariate Anaylsis
### Numeric columns
<img width="784" height="384" alt="image" src="https://github.com/user-attachments/assets/6f1559e7-d1ba-43ad-ac5f-b3223e66c07b" />
<img width="784" height="384" alt="image" src="https://github.com/user-attachments/assets/81ccf74a-9748-49d2-8a35-9a9fc6fbb2b8" />

**Observations**

- Weekly_Sales likely has a right-skewed distribution, indicating a few weeks with exceptionally high sales compared to the majority.
- Unemployment distributions are relatively tight, suggesting limited variation over the observed period.

### Categorical columns
<img width="862" height="552" alt="image" src="https://github.com/user-attachments/assets/3f76de86-8b9b-4c6d-a98d-6f25d32cd521" />

**Observations**
- The vast majority of weeks are classified as "normal week," while "holiday week" occurs much less frequently.
- This indicates that holidays are relatively rare events in the dataset compared to regular weeks.
- The imbalance between normal and holiday weeks should be considered in further analysis, as it may affect comparisons and modeling related to holiday effects on sales.

## Bi-Variate Analysis
### Categorical Vs Numeric
<img width="837" height="552" alt="image" src="https://github.com/user-attachments/assets/76e8a545-0f0e-4417-88c3-fa112c094a5e" />

**Observations**
- Sales are higher during holiday weeks compared to normal weeks.

### Numeric Vs Numeric
<img width="850" height="552" alt="image" src="https://github.com/user-attachments/assets/46e75a0d-64f6-411a-a673-d628b45f1c6c" />

**Observations**
- There is no clear relationship between fuel price and weekly sales.


### Seasonal Trends

<img width="984" height="584" alt="image" src="https://github.com/user-attachments/assets/e1446905-d512-4f80-9f2c-8a7a8f942250" />

**Observations**
- The average weekly sales show a slight downward trend over the years, indicating a gradual decrease in sales from 2010 to 2012.

<img width="984" height="584" alt="image" src="https://github.com/user-attachments/assets/4ffb2d72-25f1-4f93-9c87-871ffaff8709" />

**Observations**
- The average unemployment rate appears relatively stable over the years, with only minor fluctuations from 2010 to 2012

## Multi-variate Analysis

### Correlation Heatmap

<img width="931" height="784" alt="image" src="https://github.com/user-attachments/assets/5667ae13-491c-4113-9e3f-9f0e8e0513ed" />

**Observations**
- The correlation heatmap shows that most numeric features have weak correlations with each other. There is no strong linear relationship between weekly sales and other variables, suggesting that sales are influenced by multiple factors rather than a single dominant one.

---

# ⭐ Conclusions and Insights 

- Walmart's weekly sales exhibit a slight downward trend from 2010 to 2012, with no single external factor showing a strong linear relationship with sales.
- Holidays are associated with higher sales, but they are relatively infrequent compared to normal weeks.
- Fuel prices have gradually increased, while unemployment rates have remained relatively stable over the observed period.
- Seasonal trends are present, with certain months experiencing higher average sales, indicating the importance of seasonality in planning and forecasting.
- Most numeric features show weak correlations with each other, suggesting that Walmart's sales are influenced by a combination of factors rather than any single variable.
- Further analysis and modeling should consider the interplay of multiple variables and the impact of seasonality and holidays for more accurate forecasting and business insights.

---

# 🤝 Recommendations

- Incorporate seasonality and holiday effects into sales forecasting models to improve accuracy and support inventory planning.
- Monitor and analyze additional external factors (e.g., promotions, local events, competitor activity) that may influence sales but are not captured in the current dataset.
- Develop targeted marketing strategies for months with historically higher sales to maximize revenue opportunities.
- Continue tracking fuel prices and unemployment rates, but prioritize multi-factor models over single-variable analysis for business decisions.
- Regularly update and validate models with new data to adapt to changing trends and external influences.
- Explore store-level and department-level analyses for more granular insights and tailored operational strategies.

---

# Forecasting Future sales

<img width="1181" height="584" alt="image" src="https://github.com/user-attachments/assets/53e8415c-c754-4a12-83d4-aec521478695" />

## 📦 Installation & Setup

Ensure you have **Python 3.7+**

### Clone Repository

      git clone https://github.com/kennethnyangweso/Walmart-Sales-Analysis.git
      cd Walmart-Sales-Analysis

### Install Required Libraries
    
     pip install pandas numpy matplotlib seaborn jupyter

## 🚀 How to Run the Analysis

    jupyter notebook

    Walmart Notebook.ipynb

### Run cells in order to:

1. Load data

2. Clean & preprocess

3. Explore trends

4. Visualize insights

---
