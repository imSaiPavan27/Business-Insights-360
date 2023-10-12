# Business Insights 360

## Project Overview
AtliQ Hardware is rapidly expanding and has decided to use PowerBi for the first time to execute data analytics. As a result, the project entailed developing a Power BI dashboard for Atliq Hardware, which would provide automated data analysis for the finance, sales, marketing, and supply chain departments to improve decision-making.

## Tech Stacks
- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)


## Company's Background
AtliQ Hardware is a rapidly growing company that operates globally. They sell computer and computer accessories through three channels:
- Retailers
- Direct
- Distributors

Recently, the company faced an unforeseen loss due to the opening of a store in Latin America. To make data-driven decisions and survive in the industry, AtliQ Hardware decided to build an analytics team.

## Project Kickoff Session
The project kickoff session is where you get clarity on the project's objectives and why it's being undertaken. It's the time to ask questions and set the direction for the project.

### Project Charter 
Using a project tool lie MURAL, which helps in creating a porject charter. It outlines kep project features such
1. Project Goals
2. Project Timeline
3. Project team members
4. Project objectives
5. Project risks

## Dataset Understanding
Understanding the available data is crucial for effective analysis. Before diving into the analysis, gain a good understanding of the available data.

### Dimension Tables
- dim_customer
  - 27 distinct markets (e.g., India, USA, Spain)
  - 75 distinct customers throughout the market
  - 2 types of platforms: Brick & Mortar (Physical/offline store) and E-commerce (Online Store)
  - Three channels: Retailer, Direct, Distributors

- dim_market
  - 27 distinct markets (e.g., India, USA, Spain)
  - 7 sub-zones
  - 4 regions: APAC, EU, nan, LATAM

- dim_product
  - Divisions: P & A, Peripherals, Accessories, PC, Notebook, Desktop, N & S, Networking, Storage
  - 14 different categories (e.g., Internal HDD, keyboard)
  - Different variants available for the same product

### Fact Tables
- fact_forecast_monthly
  - Used to forecast the customer’s need in advance, leading to higher customer satisfaction and reduced storage costs.
  - Renormalized by the data engineering team for analytical work.
  - Dates of the month replaced by the start date of the month.
  - Contains forecast quantities needed by the customer.

- fact_sales_monthly
  - Similar to the fact_forecast_monthly table, but with actual sold quantities.

- gdb056
  - freight_cost: Details of travel cost and other costs for each market with fiscal year
  - gross_price: Details of gross prices with product code
  - manufacturing_cost: Details of manufacturing cost with product code and year
  - Pre_invoice_deductions: Details of pre-invoice deductions percentage for each customer with year
  - Post_invoice_deductions: Details of post-invoice deductions and other deductions

## Importing Data into PowerBi
As the database is MySQL in this project, datasets are imported from the MySQL database to PowerBi by providing the Database access credentials.

## Data Model
Data modeling is the foundation of the report. All visuals are built upon the data model. Poor data modeling can affect the overall performance of the report. In this project, a Snowfall data modeling method is followed.

## Dashboard Designing
Based on mockups received as requirements, the team will start designing visuals and creating measures as needed.

### Home View
In the Home view, all the view buttons will be available. Users will land on specific view pages by clicking the button.

- Info
- Finance View
- Sales View
- Marketing View
- Supply Chain View
- Executive View
- Products
- Support
- Overall Report

**Link to Live Interactive DashBoard**: [Power BI DashBoard](https://app.powerbi.com/view?r=eyJrIjoiYmEwOTNiNDYtMDcyZi00NWIxLThkNzYtNmQ3YWYyZDgzMTI1IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Important Techniques Learned
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

## Business-Related Terms
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
## Project Outcome
By using this report, decisions can be made based on data, and it will help answer numerous "why" questions based on various situations.
