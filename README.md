# 🚴‍♂️ AdventureWorks Sales Analysis

## 📌 Project Overview
This project presents an end-to-end data analysis and visualization of the **AdventureWorks** dataset. The goal is to extract, clean, and visualize sales performance, product trends, and customer behavior over a two-year period against the allocated budget. 

## 🛠️ Tools Used
- **SQL Server:** To extract and clean data from the Data Warehouse.
- **Power BI:** To create interactive dashboards and data visualizations.
- **Excel:** To store and manage baseline sales budget data for comparison.

## 🗂️ Data Source
The dataset used is the **AdventureWorksDW2019** Data Warehouse version provided by Microsoft Learn. The data extraction focuses explicitly on the previous two years to ensure relevance.

## 📊 Dashboards and Insights
The Power BI report is structured into three comprehensive views for different analytical needs:

### 1. Sales Overview
This main dashboard acts as an executive summary of the overall sales performance.
- **Sales by Product Category:** A donut chart illustrating sales distribution across the core product categories (Bikes, Accessories, and Clothing).
- **Budget vs. Sales by Month:** A line chart comparing actual monthly sales against the company's predefined budget over time.
- **Top 10 Customers & Products:** Bar charts highlighting the most valuable accounts and top-selling products.
- **Sales by Customer City:** A geographic map visualizing sales hotspots across North America, Europe, and Australia.

### 2. Sales by Customer
A deep dive into purchasing behaviors, making it easy to identify key clients:
- Includes a detailed matrix breaking down customer sales month over month.
- Emphasizes the Top 10 customers by sales volume and links them contextually to their geographical locations.

### 3. Sales by Product
A detailed analysis of individual product performance to help evaluate inventory success:
- Features a monthly matrix breaking down sales figures for specific product models and variations.
- Used to trace specific seasonal sales variations and precise product performance alongside geographical mapping and top product charts.

## 📁 Repository Structure
- `analysis.sql`: Contains the SQL queries used to extract and clean the `DimDate`, `DimCustomer`, `DimProduct`, and `FactInternetSales` tables from the warehouse.
- `DimDate.csv`, `portfolio_1-data_table-DimCustomer.csv`, `DimProduct.csv`, `FactInternetSales.csv`: The cleaned datasets extracted via the SQL script.
- `SalesBudget.xlsx`: The initial budget data used to compare actuals vs. budget.
- `portfolio_1-project-visualization_powerbi.pbix`: The interactive Power BI project file.
- `visualization.pdf`: A static snapshot/export of the three Power BI dashboard pages.

## 🚀 How to Use
1. Clone the repository to your local machine.
2. Download the PBIX file (`portfolio_1-project-visualization_powerbi.pbix`) and open it in **Power BI Desktop** to view or iterate on the interactive dashboard.
3. Alternatively, view the static snapshots of the dashboards in `visualization.pdf`.
4. The SQL code in `analysis.sql` can be executed directly on the AdventureWorksDW2019 database if you'd like to recreate the data extracts or query real-time data yourself.
