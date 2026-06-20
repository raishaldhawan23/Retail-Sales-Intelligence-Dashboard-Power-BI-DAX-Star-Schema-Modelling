# 📊 Live Interactive Dashboard: https://raishaldhawan23.github.io/Retail-Sales-Intelligence-Dashboard-Power-BI-DAX-Star-Schema-Modelling/
## *Click the link above to open the fully interactive Power BI report, where you can click filters, slicers, and explore the live metrics.*


# Retail-Sales-Intelligence-Dashboard-Power-BI-DAX-Star-Schema-Modelling

## 1. Executive Summary

This project presents an end-to-end Business Intelligence solution built in Power BI to analyse retail sales performance across stores, brands, products and geographies.

The project integrates eight separate business datasets covering customers, orders, products, stores, currencies and sales transactions into a unified star schema model. Using DAX calculations, Power Query transformations and interactive visualisations, the dashboard provides operational, analytical and executive-level views of business performance.

The analysis focuses on answering key business questions:

1. Which stores generate the highest revenue?
2. Which brands and categories contribute most to sales?
3. How has revenue changed over time?
4. Which countries and continents drive business growth?
5. Is recent performance improving or declining?

The final solution delivers a self-service dashboard enabling business users to explore revenue, profit, quantity sold and growth trends through interactive filtering and drill-down capabilities.

## 2. Project Background

### Business Context

Retail businesses generate large volumes of transactional data across products, stores, customers and geographies.

However, raw data alone provides little value unless decision-makers can answer questions such as:

- Which stores are performing best?
- Which products drive the majority of revenue?
- Are revenues growing or declining?
- Which regions should receive more investment?
- Which categories have the highest volume but lowest profitability?

The challenge in this project was to transform multiple disconnected datasets into a single business intelligence solution that supports operational decisions, analytical investigations and executive reporting.

### Business Objectives

The dashboard was designed to:

- Integrate 8 business datasets into a unified data model.
- Create an interactive filtering experience for end users.
- Identify top-performing stores by revenue.
- Analyse brands, categories and products by revenue and quantity sold.
- Track monthly, quarterly and yearly revenue trends.
- Evaluate revenue performance across countries and continents.
- Provide executives with growth and profitability insights.

## 3. Data Architecture

The project integrates:

| Table             | Purpose                        |
| ----------------- | ------------------------------ |
| Customer          | Customer information           |
| Product           | Product hierarchy              |
| Orders            | Order header information       |
| OrderRows         | Transaction-level sales        |
| Store             | Geography and store details    |
| Sales             | Revenue information            |
| Currency Exchange | Exchange rates                 |
| Date              | Calendar and time intelligence |

### Data Model

<img width="1187" height="776" alt="image" src="https://github.com/user-attachments/assets/2dfa152a-69c8-4c91-8381-7c60ec5145fb" />


#### A Star Schema was implemented:

#### Fact Table

- OrderRows

#### Dimension Tables

- Date
- Customer
- Product
- Store
- Currency

This model improves:

- Query performance
- Scalability
- DAX calculations
- Time intelligence functions
- Filter propagation

## 4. Dashboard Structure

The dashboard was divided into three perspectives:

### a. Operations View

<img width="1451" height="797" alt="image" src="https://github.com/user-attachments/assets/e2f2b149-1047-4294-8148-b8ffc08bbfc2" />


Designed for operations teams to monitor:

- Revenue
- Profit
- Quantity Sold
- Top Brands
- Product Performance
- Category Performance

Business question:

Which products and brands contribute the most to revenue?

### b. Analytics View

<img width="1447" height="800" alt="image" src="https://github.com/user-attachments/assets/c3f2d80d-f55c-4db1-9ad0-3f2fc94a4b4d" />


Designed for analysts to investigate:

- Monthly revenue trends
- Yearly trends
- Revenue vs Quantity relationships
- Year-over-Year growth

Business question:

Is the business growing, and which categories drive growth?

### c. Executive View

<img width="1440" height="797" alt="image" src="https://github.com/user-attachments/assets/d51a9b94-402f-49ae-af3f-860e35f2c9ac" />


Designed for leadership teams.

Provides:

- Country-wise revenue
- Continent performance
- Quarterly revenue breakdown
- Top-performing stores

Business question:

Which regions and channels deserve more investment?

## 5. Key Findings

### 1. Online Channels Dominate Revenue

<img width="1702" height="762" alt="image" src="https://github.com/user-attachments/assets/c7151ad9-a658-4d05-98df-25431b60db4a" />


The Online Store generated substantially more revenue than individual physical stores.

This suggests:

- Strong digital purchasing behaviour.
- Opportunities for further investment in e-commerce.
- Potential overdependence on a single sales channel.

### 2. Computers Drive Business Performance

<img width="1731" height="762" alt="image" src="https://github.com/user-attachments/assets/6819f978-270f-4f06-b436-8b1298854caa" />


The Computers category generated:

- Highest revenue
- Highest sales quantity
- Largest contribution to total sales

Meanwhile:

- Audio
- Games & Toys

contributed relatively little revenue.

This indicates an unequal revenue distribution across categories.

### 3. North America Drives Most Revenue

<img width="1732" height="765" alt="image" src="https://github.com/user-attachments/assets/d3ad086c-fd77-4152-90f9-54649e08dcb2" />


North America accounted for the largest share of revenue across all years.

Europe ranked second, while Australia contributed a comparatively smaller proportion.

This highlights:

- Regional concentration risk.
- Opportunities to expand underperforming markets.

### 4. Revenue Declined Significantly in FY2024

The dashboard showed:

#### *YoY Growth = -78.81%*

However, this is likely explained by:

- Partial FY2024 data availability.
- Only Q1 sales are being included.

Therefore:

The decline should not immediately be interpreted as business deterioration.

It is a data completeness consideration rather than a confirmed business issue.

### 5. Data Quality Issues Were Exposed

Several transactions were associated with:

StoreKey = 999999

But no corresponding store existed in the Store dimension.

This resulted in:

- Blank store names
- Revenue assigned to unknown entities

Instead of removing these records, they were deliberately retained to expose a real business data quality issue.

## Tools and Analytical Capabilities
Tools
- Power BI
- Power Query
- DAX
- Power Query M

Data Modelling & Analytics
- Star Schema Modelling
- Data Modelling
- Time Intelligence
- Data Cleaning & Validation

Frameworks & Methodologies
- CRISP-DM
