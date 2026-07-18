## ☕ **Coffee Sales Data Analytics Dashboard (Excel)**

An end-to-end Excel analytics project that cleans raw coffee sales data, joins it across multiple tables using XLOOKUP, and turns it into an interactive Pivot Table + Pivot Chart dashboard with slicers and timeline for business exploration.

**Project Overview**

The workbook takes three raw, disconnected data sources and turns them into a single clean dataset, then builds a dashboard on top of it so a non-technical stakeholder (e.g. a sales manager) can filter and explore the numbers themselves — no formulas required on their end.

**Dataset**

The workbook contains 1,000 coffee orders across three linked tables:
- **Orders**
  - **Description:** Raw transaction-level order data
  - **Key Columns:** Order ID, Order Date, Customer ID, Product ID, Quantity, Sales

- **Customers**
  - **Description:** Customer master data
  - **Key Columns:** Customer ID, Name, Email, Address, Country, Loyalty Card

- **Products**
  - **Description:** Product master data
  - **Key Columns:** Product ID, Coffee Type, Roast Type, Size, Unit Price, Profit
  
**Coverage**
- **Countries:** United States, United Kingdom, Ireland
- **Coffee Types:** Arabica, Excelsa, Robusta, Liberica
- **Roast Types:** Light, Medium, Dark
- **Sizes:** 0.2 kg, 0.5 kg, 1.0 kg, and other available package sizes

**Data Cleaning & Preparation**

Before analysis, the raw data was cleaned and standardized:

- Removed inconsistent formatting across the **Orders**, **Customers**, and **Products** sheets.
- Identified and removed duplicate records to improve data quality.
- Standardized coffee type and roast type abbreviations (e.g., `Ara`, `Rob`) into readable names (e.g., `Arabica`, `Robusta`).
- Verified that **Customer ID** and **Product ID** were consistent across all tables to ensure accurate data joins using **XLOOKUP**.
- Prepared a clean, analysis-ready dataset for Pivot Tables, Pivot Charts, and dashboard creation.

**Data Integration Using XLOOKUP & INDEX**

Since the **Orders**, **Customers**, and **Products** data were stored in separate tables, **XLOOKUP** and **INDEX + MATCH** were used to combine them into a single analysis-ready dataset.

- Used **XLOOKUP** to retrieve customer and product information by matching **Customer ID** and **Product ID**.
- Used **INDEX + MATCH** for dynamic lookups based on row and column references.
- Combined transactional, customer, and product data into one clean dataset for analysis.

**Pivot Tables & Pivot Charts**

Three Pivot Tables were created to summarize and visualize the sales data:

- **Sales by Coffee Type & Roast** – Summarizes total sales by coffee type (Arabica, Excelsa, Liberica, Robusta) and roast type (Light, Medium, Dark).
- **Top 5 Customers by Sales** – Identifies the highest-value customers based on total sales.
- **Sales by Country** – Compares total sales across the United States, United Kingdom, and Ireland.

**Slicers & Timeline**
Interactive **Slicers** and a **Timeline** were added to make the dashboard fully interactive.

**Slicers**
Users can instantly filter the dashboard by:
- Country
- Coffee Type
- Roast Type
- Loyalty Card Status (Yes/No)

**Timeline**
An interactive **Timeline** linked to the Order Date field allows users to filter sales by:
- Year
- Quarter
- Month
- Day

📈 **Dashboard**

All pivot charts, slicers and timeline are combined into a single Dashboard sheet — a one-page view designed to be opened by someone who isn't comfortable digging through raw data, giving them an instant snapshot of sales performance by product, geography, and customer.

🚀 **How to Use**

- Download coffeeOrdersData_with_dashboard.xlsx and open it in Excel (2021 or Microsoft 365 recommended for full XLOOKUP/slicer support)
- Start on the Dashboard sheet for the high-level summary
- Use the slicers to filter by country, coffee type, roast, or loyalty status
- Explore the orders, customers, and products sheets to see the underlying cleaned and joined data
