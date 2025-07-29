# Walmart-Sales-Analysis
# 🧠 Business Understanding

## 🔹 1. Project Overview
Walmart, one of the largest retail chains in the world, operates hundreds of stores across various locations and departments. Analyzing its historical sales data can help uncover valuable insights into store performance, the impact of external factors (like holidays and fuel prices), and customer purchasing behavior. 

The goal of this project is to analyze and visualize Walmart’s sales data to support data-driven decision-making across store management, inventory planning, and marketing.

---

## 🔹 2. Problem Statement
Walmart’s sales performance varies across different stores and time periods, and is influenced by external factors such as holidays, fuel prices, and weather conditions. However, decision-makers lack a consolidated view of these insights.

**How can we identify patterns, trends, and anomalies in Walmart’s historical sales data to support strategic planning and operational decisions?**

---

## 🔹 3. Project Objectives
- Perform exploratory data analysis (EDA) to understand sales patterns and key influencing factors.
- Identify top-performing stores and departments.
- Analyze the impact of holidays and seasons on sales.
- Build interactive dashboards (Python, Tableau, Power BI) for decision-makers.
- *(Optional)* Forecast future sales based on historical patterns.

---

## 🔹 4. Metrics for Success

### ✅ Descriptive Insight Metrics:
- Clear identification of trends, outliers, and seasonality.
- Top/bottom performing stores and departments.
- Correlation of external factors (like holidays and fuel prices) with sales.



### ✅ Predictive Metrics:
- Accuracy of sales forecasts (e.g., RMSE or MAPE).
- Precision in anomaly detection or classification tasks if any.

# 📊 Data Understanding Summary

## 🔹 Dataset Overview
- **Total Records:** 6,435
- **Columns:** 8


---

## 🔹 Columns & Observations

| Column           | Type    | Notes |
|------------------|---------|-------|
| `Store_Number`   | int64   | Unique store identifier |
| `Date`           | object  | Needs conversion to datetime |
| `Weekly_Sales`   | object  | Stored as string with commas → needs conversion to numeric |
| `Holiday_Flag`   | int64   | 0 = Normal week, 1 = Holiday week |
| `Temperature`    | float64 | Average weekly temperature |
| `Fuel_Price`     | float64 | Fuel cost per gallon |
| `CPI`            | int64   | Consumer Price Index (note: should be float, also column name has extra space) |
| `Unemployment`   | float64 | Unemployment rate (%) |

---

## 🔹 Immediate Actions Needed
1. 🔄 Convert `Weekly_Sales` from string to numeric (remove commas).
2. 📅 Convert `Date` to datetime format.
3. 🧹 Rename `" CPI"` column to `"CPI"` (remove leading space).
4. 📈 Proceed to univariate and bivariate EDA.

# Exploratory Data Analysis

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


