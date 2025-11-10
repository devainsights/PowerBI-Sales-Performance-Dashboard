# 📊 Power BI – Sales Performance Dashboard

### ✅ Objective
To analyze company sales and derive insights about:
- Total revenue
- Top performing product lines
- High revenue regions
- Monthly sales trend

### 📁 Dataset
Source: Kaggle – Sample Sales Data  
Link: https://www.kaggle.com/datasets/kyanyoga/sample-sales-data

### 🔧 Tools & Skills Used
- Power BI Desktop
- Power Query (Data Transformation)
- DAX (Measures: Total Sales, Total Orders, Avg Order Value)
- Data modeling
- Dashboard design principles

### 🧠 Business Questions Answered
| No | Business Question |
|----|------------------|
| 1 | What is the total sales revenue? |
| 2 | Which product line contributes highest sales? |
| 3 | Which region generates maximum revenue? |
| 4 | What is the monthly trend of sales? |
| 5 | Who are the top customers based on revenue? |

### 🧮 Measures Used (DAX)
Total Sales = SUM('sales_data_sample'[SALES])
Total Orders = DISTINCTCOUNT('sales_data_sample'[ORDERNUMBER])
Average Order Value = [Total Sales] / [Total Orders]
Monthly Sales = CALCULATE([Total Sales], DATESMTD('sales_data_sample'[ORDERDATE]))
