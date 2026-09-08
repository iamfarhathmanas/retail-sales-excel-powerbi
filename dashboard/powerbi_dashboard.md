# Power BI Dashboard Specification

## Page 1 — Executive Overview
- KPI Card: Total Revenue
- KPI Card: Total Profit
- KPI Card: Profit Margin
- KPI Card: Units Sold
- Line chart: Monthly Revenue and Profit
- Bar chart: Revenue by Region

## Page 2 — Product & Channel
- Bar chart: Revenue by Product
- Column chart: Profit by Product
- Matrix: Channel, Revenue, Profit, Margin
- Slicers: Date, Region, Product, Channel

## Suggested Measures
```DAX
Total Revenue = SUM(RetailSales[Revenue])
Total Profit = SUM(RetailSales[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Revenue])
Units Sold = SUM(RetailSales[Quantity])
```
