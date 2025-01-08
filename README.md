# AtliQ-Hardware-Business-Insights-360

## Project Overview

AtliQ Hardware is growing rapidly in recent years, and they have decided to implement data analytics using Power BI to surpass their competitors in the market and make data-driven decisions. This project answers stakeholders' questions across finance, sales, marketing, and supply chain.

I worked on this project by following the Codebasics Power BI Course. Link to the course is [here](https://codebasics.io/bootcamps/dashboard/data-analytics-bootcamp-with-practical-job-assistance).


---

## Tech Stacks

- SQL
- Power BI Desktop
- Excel
- DAX Language
- DAX Studio (for optimizing the report)
- Project Charter File

---


---

## Power BI Techniques Learned

- Asking the right questions before starting the project
- Creating calculated columns and measures using DAX language
- Data modeling and visualization techniques
- Using bookmarks, page navigation, and dynamic titles
- Power BI Service setup and automation (e.g., auto-refresh with gateways)
- Collaboration and workspace management
- And much more! 😅

---

## Business-Related Terms

- Gross Price
- Pre-Invoice Deductions
- Post-Invoice Deductions
- Net Invoice Sale
- Gross Margin
- Net Sales
- Net Profit
- Cost of Goods Sold (COGC)
- YTD (Year to Date)
- YTG (Year to Go)

---

## Dataset Understanding

This project uses data from multiple tables:
1. **Dimension Tables**: Contain static data like customer and product details.
2. **Fact Tables**: Contain transactional data for sales, forecasts, and costs.
3. 
- gdb041:
    - dim_customer
        - **27** distinct markets (ex India, USA, spain)
        - **75** distinct customers thorough out the market
        - **2** types of platforms
            - Brick & Motors - Physical/offline store
            - E-commerce - Online Store (Amazon, flipkart)
        - Three channels
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - **27** distinct markets (ex India, USA, spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
    - dim_product
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
        - This table is used to forecast the customer’s need in advance, which can help in
            - Higher customer satisfaction
            - Reduced cost in warehouses for storage purpose
        - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
        - All the date of the month will be replaced by the start date of the month
        - It will have all the column names and in the end it will have the forecast quantity need of the customer
    - fact_sales_monthly
        - This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
- gdb056
    - freight_cost
        - This table has details of travel cost and other cost for each market with fiscal year
    - gross_price
        - Has the details of gross prices with product code
    - manufacturing_cost
        - Has the details of manufacturing cost with product code with year
    - Pre_invoice_dedutions
        - Has the details of pre invoice deductions percentage for each cutomer with year
    - Post_invoice_deductions
        - Post invoice deductions and other deductions details



---

## Importing Data into Power BI

The datasets are imported from a MySQL database into Power BI. Database credentials were provided for secure access.  

---

## Data Model and Dashboard

We followed a snowflake data modeling approach for this project. For detailed visuals of the data model and the interactive dashboards:  
- **Full Report**: [Report File](https://app.powerbi.com/view?r=eyJrIjoiZGRmZjY4ZGEtYzhmMC00MWE3LWI5YWItM2E5MzExYzRjZGI2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9).

---

## Project Outcome

By using this report, stakeholders can make data-driven decisions and address "why" questions across various business scenarios.  

For a visually appealing showcase, visit the **Live Report on Novy Pro**:  
[**Live Report Link**](#) ← **Replace this with your Novy Pro link**
