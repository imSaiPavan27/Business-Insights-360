# Business Insights 360


## Project Overview
AtliQ Hardware is experiencing rapid growth and has decided to implement data analytics using PowerBi for the first time. The aim is to outperform competitors in the market and make data-driven decisions. This project is expected to provide insights into various aspects, including finance, sales, marketing, and the supply chain.

**Live Report Link**: [Link to Live Report](#)

## Tech Stacks
- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)

## Project Charter File
- [Link to Project Charter File](#)

## PowerBI Techniques Learned
- What are all the questions that should be asked before starting the project?
- Creating calculated columns
- Creating measures using DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using the divide function to prevent zero division errors
- Creating date tables using M language
- Dynamic titles based on applied filters
- Using KPI indicators
- Conditional formatting of values in visuals using icons or background color
- Data validation techniques
- PowerBi services
- Publishing reports to PowerBi services
- Setting up a personal gateway for auto data refresh
- PowerBi App creation
- Collaboration, workspace, access permissions in PowerBi services

## Business-Related Terms
- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGC – cost of goods sold
- YTD – Year to Date
- YTG – Year to Go
- Direct
- Retailer
- Distributors
- Consumer

## Company's Background
AtliQ Hardware is a rapidly growing company that operates globally. They sell computer and computer accessories through three channels:
- Retailers
- Direct
- Distributors

Recently, the company faced an unforeseen loss due to the opening of a store in Latin America. To make data-driven decisions and survive in the industry, AtliQ Hardware decided to build an analytics team.

## Project Kickoff Session
The project kickoff session is where you get clarity on the project's objectives and why it's being undertaken. It's the time to ask questions and set the direction for the project.

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

**You can find the full report file here**: [Link to Full Report](#)

## Project Outcome
By using this report, decisions can be made based on data, and it will help answer numerous "why" questions based on various situations.
