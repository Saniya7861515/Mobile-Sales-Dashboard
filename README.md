# Mobile-Sales-Dashboard
This project presents a Mobile Sales Dashboard built in Power BI using Excel data. It provides clear and interactive visualizations to help understand mobile sales performance across India, analyze customer behavior, and track business KPIs.
##  Key Features of the Dashboard

### 1. **Dashboard Page**
- **KPIs Displayed**:
  - Total Sales: 769M
  - Total Quantity Sold: 19K
  - Total Transactions: 4K
  - Average Price per Mobile: ₹40.11K
- **Visuals**:
  - Map of India – Sales by City
  - Line Chart – Quantity sold by Month
  - Pie Chart – Transactions by Payment Method
  - Bar Charts:
   - Ratings (Good, Average, Poor)
   - Total Sales by Mobile Model
    - Total Sales by Day of the Week
- **Filters**: Mobile Model, Brand, Payment Method

### 2. **MTD (Month-to-Date) Report Page**
- MTD sales growth chart (daily trend for the month)
- KPIs for selected month: Sales, Quantity, Transactions, Avg. Price
- Filters: Month, Mobile Model, Payment Method

### 3. **Same Period Last Year Comparison Page**
- Year-over-Year (YoY) Sales Comparison by:
  - Year
  - Quarter
  - Month
- Bar Charts – Current vs Previous Year sales
- Table – Quarterly total sales with previous year's data
---

## Tools & Techniques Used

| Tool/Feature            | Description |
|-------------------------|-------------|
| **Power BI Desktop**    | Dashboard design, interactive visuals |
| **Excel**               | Data Source (uploaded file) |
| **Power Query Editor**  | Data cleaning, column transformation, data types |
| **DAX (Data Analysis Expressions)** | Calculated Columns and Measures |
---

## Important DAX Formulas Used

- **Total Sales** =  SUMX('Mobile _Sales_ Data','Mobile _Sales_ Data'[Units Sold]*'Mobile _Sales_ Data'[Price Per Unit])

- **Average Price** =  AVERAGE('Mobile _Sales_ Data'[Price Per Unit])

- **MTD Sales** = TOTALMTD([Total_Sales],custom_calendar[Date].[Date])

- **Same Period Last Year** = CALCULATE([Total_Sales],
 SAMEPERIODLASTYEAR(custom_calendar[Date]))
---
## Insights from the Dashboard

- High sales in cities like **Mumbai, Delhi, Ranchi**.
- Most popular mobile models: **iPhone SE**, **OnePlus Nord**, **Galaxy Note 20**.
- Majority of transactions via **UPI** and **Credit Card**.
- Sales peak on **Monday and Friday**.
- Year-on-Year sales show growth from **2022 to 2024**.

## 🗂 Project Files Included
- Data: https://github.com/Saniya7861515/Mobile-Sales-Dashboard/blob/main/Day%20-%2030%20-%20Mobile%20Sales%20Data.xlsx
- Dashboard:https://github.com/Saniya7861515/Mobile-Sales-Dashboard/blob/main/Dashboard%20of%20Mobile%20Sales.pbix
- Images:


