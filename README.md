# Worksforce_And_Sales_Analysis
# Workforce & Sales Intelligence Analysis

## Project Overview

Workforce & Sales Intelligence Analysis is an Excel-based business analytics project focused on evaluating sales performance, profitability, customer behavior, product performance, regional performance and order operations.

The project uses multiple datasets and advanced Excel techniques to transform raw transactional data into actionable business insights through KPIs, PivotTables, interactive slicers and dashboard visualizations.

---

## Business Objective

The primary objective of this analysis was to:

- Evaluate overall sales and profitability
- Identify high-performing regions and product categories
- Analyze customer purchasing behavior
- Monitor regional sales performance against targets
- Identify high-value customers and products
- Analyze payment methods and order status
- Detect and correct data-quality issues
- Build an interactive management dashboard

---

## Dataset

The project consists of multiple data sources:

### AmazonSales
Contains transactional information including:

- Order ID
- Order Date
- Delivery Date
- Cancel Date
- Customer ID
- Product ID
- Region
- Sale Price/Unit
- Quantity
- Total Amount
- Payment Method
- Delivery Status
- Fulfillment Partner

### ProductMaster

Contains:

- Product ID
- Product Name
- Category
- Cost Price
- Product Description

### CustomerMaster

Contains:

- Customer ID
- Customer Name
- Customer Type
- City
- State

### RegionGoals

Contains regional sales targets used for target-performance analysis.

---

## Data Preparation

The raw transaction data was validated and cleaned before analysis.

### Major Data Quality Issue

The original `Total Amount` field contained the value `44` across all 100 transactions, which was inconsistent with the available unit price and quantity fields.

The field was recalculated using:

`Total Amount = Sale Price/Unit × Quantity`

This ensured that revenue calculations were based on the actual transaction values.

### Additional Transformations

- Integrated product information using XLOOKUP
- Integrated customer information using VLOOKUP
- Added product cost information
- Calculated transaction-level profit
- Extracted month information from order dates
- Validated order status, payment method and regional fields
- Created an analysis-ready dataset

---

## Key KPIs

| KPI | Result |
|---|---:|
| Total Orders | 100 |
| Total Sales | $35,258 |
| Total Profit | $2,387 |
| Units Sold | 312 |
| Average Order Value | $352.58 |
| Profit Margin | 6.77% |

---

## Key Business Insights

### Regional Performance

North was the strongest-performing region with:

- $10,491 sales
- $748 profit

West ranked second with $8,359 sales and $601 profit.

This indicates that North is currently the strongest regional market.

---

### Product Category Performance

Electronics was the strongest category:

- $15,209 sales
- $1,043 profit

Home ranked second with $10,951 sales and $742 profit.

Electronics contributed approximately 44% of total sales and profit.

---

### Product Performance

The Smartphone was the highest-performing individual product:

- $9,644 sales
- $656 profit

It generated approximately 27% of total sales, indicating significant sales concentration around a single high-performing product.

---

### Customer Performance

Liam Walker was the highest-value customer with:

- $5,299 sales

Other high-value customers included Elijah Lewis and Noah Wilson.

This suggests an opportunity to develop targeted customer retention and loyalty strategies.

---

### Payment Method

Credit Card generated the highest sales value at:

- $9,398

Debit Card followed with:

- $8,348

Understanding payment preferences can help optimize customer experience and payment-channel strategies.

---

## Excel Techniques Used

- XLOOKUP
- VLOOKUP
- SUMIFS
- COUNTIFS
- IF/IFERROR
- Date and text functions
- Calculated columns
- PivotTables
- KPI calculations
- Conditional formatting
- Data validation
- Interactive slicers
- Dashboard creation
- Data integration
- Business analysis

---

## Dashboard

The interactive dashboard was designed to provide management with a quick view of:

- Total Sales
- Total Profit
- Orders
- Average Order Value
- Regional Performance
- Product Category Performance
- Top Products
- Top Customers
- Payment Method Performance
- Delivery Status
- Regional Target Performance

Interactive slicers allow users to dynamically filter the analysis and investigate specific business segments.

---

## Business Recommendations

1. Prioritize Electronics due to its leading contribution to sales and profit.
2. Maintain strong customer and inventory strategies in the North region.
3. Monitor dependence on high-performing products such as the Smartphone.
4. Develop retention strategies for high-value customers.
5. Use regional target analysis to identify underperforming markets.
6. Monitor cancelled and in-transit orders to improve operational performance.

---

## Tools

**Microsoft Excel**

- Advanced Excel Formulas
- PivotTables
- Slicers
- KPI Analysis
- Data Cleaning
- Data Validation
- Dashboarding
- Business Intelligence

---

## Outcome

The project transformed raw transactional data into an interactive business intelligence solution, enabling management to monitor sales, profitability, customer behavior, product performance and regional performance through a single analytical dashboard.
