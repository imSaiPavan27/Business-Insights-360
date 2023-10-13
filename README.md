
# Business Insights 360

## 1. Project Overview
AtliQ Hardware is rapidly expanding and has decided to use PowerBi for the first time to execute data analytics.The Business Insights 360 dashboard should be built using Microsoft Power BI. This multi-functional dashboard should be tailored in such a way that it should provide AtliQ Hardware with vital insights into their many departments such as Finance, Sales, Marketing, and Supply Chain on a worldwide scale. 

### About AtliQ Hardware
AtliQ Hardware is a rapidly growing company that operates globally. They sell computer and computer accessories through three channels:
- Retailers
- Direct
- Distributors

Recently, the company faced an unforeseen loss due to the opening of a store in Latin America. To make data-driven decisions and survive in the industry, AtliQ Hardware decided to build an analytics team.

## 2. Project Planning
The project planning session is where you get clarity on the project's objectives and why it's being undertaken. It's the time to ask questions and set the direction for the project and create a **Project Charter**

### Project Charter 
Using a project tool lie **MURAL**, which helps in creating a porject charter. It outlines kep project features such
1. Goals
2. Timeline
3. Team members
4. Objectives
5. Risks

## 3. Import & Explore Data
### A. Importing Data into SQL
Importing the AtliQ's data into the MySQL Workbench. The data includes both fact and dimension tables.

### B. Using SQL to Explore Data
Understanding the available data is crucial for effective analysis. Before diving into the analysis, gain a good understanding of the available data. 

#### Dimension Tables
- **dim_customer**
  - 75 distinct customers throughout the market
  - 2 types of platforms: Brick & Mortar (Physical/offline store) and E-commerce (Online Store)
  - Three channels: Retailer, Direct, Distributors
- **dim_market**
  - 27 distinct markets (e.g., India, USA, Spain)
  - 7 sub-zones
  - 4 regions: APAC, EU, nan, LATAM
- **dim_product**
  - Divisions: P & A, Peripherals, Accessories, PC, Notebook, Desktop, N & S, Networking, Storage
  - 14 different categories (e.g., Internal HDD, keyboard)
  - Different variants available for the same product

#### Fact Tables
- **fact_forecast_monthly**
  - Used to forecast the customer’s need in advance, leading to higher customer satisfaction and reduced storage costs.
  - Renormalized by the data engineering team for analytical work.
  - Dates of the month replaced by the start date of the month.
  - Contains forecast quantities needed by the customer.
- **fact_sales_monthly**
  - Similar to the fact_forecast_monthly table, but with actual sold quantities.

#### Miscellaneous Data 
  - **freight_cost**: Details of travel cost and other costs for each market with fiscal year
  - **gross_price**: Details of gross prices with product code
  - **manufacturing_cost**: Details of manufacturing cost with product code and year
  - **Pre_invoice_deductions**: Details of pre-invoice deductions percentage for each customer with year
  - **Post_invoice_deductions**: Details of post-invoice deductions and other deductions

**Note**: The Database which has both fact and dimension tables, consists of more than 1.4 million records of different products, customers, purchases, etc..

### C. Import data to Power BI
After exploring the data, we now connect and load the AtliQ's data from MySQL database to the Power BI.

## 4. Data Modelling
Data modeling is the foundation of the report. All visuals are built upon the data model. Poor data modeling can affect the overall performance of the report. 

After importing data into the Power BI, the following procedures are to be followed:
1. Cleaning, formatting and transforming the data using power query
2. Establishing relationships among the  tables, employing either **Star Schema** or the **Snow Flake** methodology.
3. Subsequently, conducting data validation against the benchmarks set by the stakeholders

## 5. Dashboard Designing
Based on mockups received as requirements, the team will start designing visuals and creating measures as needed.

### Home View
In the Home view, all the view buttons will be accessible. Users will land on specific view pages by clicking the button and you can navigate to the certain view.

The different views are:

| Views | Description |
| ------ | ----------- |
| Info  | It gives an overview of the fundamental data generation process and used to notify updates |
| Finance | It enables users to analyze P&L statements ,understanding the net sales and expolring other fiscal metrics |
| Sales  | It shows a detailed analysis of sales efforts, supporting in improvement of strategy and informed decison making |
| Marketing | It shows the customer engagement, impact of the product and market research which empowers stakeholders to redefine their marketing strategy |
| Supply Chain  | It provides insights into inventory levels, order fulfillments and logistics which facilitates streamlined operations |
| Exective  | It presents some of the important KPI's and tracks market shares trends |
| Support  | It porvides support measures for the customers who are facing issues |

## 6. Project Outcomes
By using this report, decisions can be made based on data, and it will help answer numerous "why" questions based on various situations.

The learnings from this porject:

### A. Important Techniques 
- Getting started with Exploratory Data Analysis using SQL
- Making connections between SQL and Power BI
- Shaping data with Power Query
- Building data models
- Crafting Date Tables using M language
- Crafting Measures with DAX
- Understanding the nuances of Filter Context
- Using Bookmarks for seamless switching between visuals
- Navigating pages through buttons
- Applying Conditional Formatting for more engaging insights
- Making the most of KPI Indicators
- Utilizing Generated Columns effectively
- Improving performance through DAX Studio optimization

### B. Business-Related Terms
- Net sales
- Net Profit
- Net-invoice sales
- Gross price
- Gross margin
- Pre-invoice deductions
- Post-invoice deductions
- COGS ( Cost of goods sold )
- YTD ( Year to do )
- YTG ( Year to go )

### C. Tech Skills
- MySQL
- PowerBi Desktop
- MS Excel
- DAX language
- DAX studio (for optimizing the report)

### **Link to Business Insights 360 Presentaion** : [Linkedin Post](https://www.linkedin.com/feed/update/urn:li:activity:7117530718058008576/)
### **Link to Live Interactive DashBoard**: [Power BI DashBoard](https://app.powerbi.com/view?r=eyJrIjoiYmEwOTNiNDYtMDcyZi00NWIxLThkNzYtNmQ3YWYyZDgzMTI1IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)
