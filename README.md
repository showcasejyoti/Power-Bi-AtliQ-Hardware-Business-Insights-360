# Power-Bi-AtliQ-Hardware-Business-Insights-360


## 🧾 Project Overview

AtliQ Hardware is a global electronics company specializing in computers, peripherals, and accessories. In recent years, the company has significantly expanded its operations worldwide. With this rapid growth, the complexity of business challenges has also increased.
To tackle these challenges and promote data-driven decision-making, AtliQ Hardware has hired a dedicated Data Analytics team. While the company previously relied on Excel for reporting, the growing scale of operations has made Power BI the preferred tool for advanced data visualization and reporting.
This project aims to provide stakeholders with actionable insights across key business domains such as Finance, Sales, Marketing, and Supply Chain. The ultimate goal is to ensure greater data transparency and support strategic decision-making through interactive Power BI dashboards.

The entire project has provided end to end experience. I worked on this project by following the Codebasics PowerBi Course, Link to the course is [here](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project)


## 🔗 Live Dashboard Link
 [Click here to view the dashboard](https://app.powerbi.com/groups/869ba0a8-e859-477e-ae6f-40de64dc726f/reports/1b416459-51f8-45ba-96d3-374429b37711/d432794ba64090d60710?experience=power-bi)
 

## 🧠 Learnings

### 🧰 Tech Stacks

- PowerBi Desktop
- My SQL
- Excel
- DAX language
- DAX studio (for performance optimization- VertiPaq Analyser)
- Project Charter (Mural)

### 🧹 Data Collection
- Data Catalog
-	Unzip & uncompress the sql text
-	My SQL (import the database)

### 🛠 Power BI Techniques

#### &nbsp;&nbsp;&nbsp; Data Importing
- MySQL
- Excel
- Other external sources
  
####	&nbsp;&nbsp;&nbsp; Data Preparation
- Data cleaning in Power Query
- Creating calculated columns in Power Query
- Creating a Date Table using M language
  
#### &nbsp;&nbsp;&nbsp; Data Modeling
-	Building Data Model
-	Creating calculated columns in Power BI
  
####	&nbsp;&nbsp;&nbsp; DAX Measures & Expressions
-	Creating measures using DAX
-	Numeric parameters as dynamic slicers
-	Field parameters to switch visual fields
  
####	&nbsp;&nbsp;&nbsp; Visual Customization
-	Adding dynamic titles and labels based on user selection
-	Conditional formatting: icons, background colors, and data bars
-	Using tooltips to show trends
-	Merging donut charts and bar charts for better interactivity
  
#### &nbsp;&nbsp;&nbsp; 	Navigation & Interactivity
-	Adding page navigation with buttons
-	Using the Selection Pane and Bookmarks for pop-up notifications
-	Toggling between visuals using Bookmarks
-	Applying different types of Filters

####	&nbsp;&nbsp;&nbsp; Power BI Features
-	Utilizing updated visuals: New Card, Button Slicer

####	&nbsp;&nbsp;&nbsp; Power BI Service
-	Publishing reports
-	Exporting reports
-	Sharing with access control
-	Creating apps
-	Using endorsements
-	Collaboration
-	Getting insights
-	Managing gateways and data connections

### 📊 Business Metrics
-	Gross Sales
-	Pre Invoice Deduction
-	Net Invoice Sales
-	Post Invoice Discount
-	Post Invoice other Deduction
-	Total Post Invoice Deduction
-	Net Sales
-	Total COGS: Manufacturing Cost, Freight Cost, Other Cost
-	Gross Margin
-	Operational Expense: Ads & Promotion, Other Operational Expenses
-	Net Profit
-	YTD - Year To Date
-	YTG- Year To Go
-	Net Error
-	Absolute Error
-	Forecast Accuracy
-	Revenue Contribution

   
 	Following is a schema of Bussiness Metrics for better understanding :

   ![Business metrics schema](https://github.com/user-attachments/assets/b3127c2b-a643-4a76-b35a-727a38074474)

   
### 📚 Terminology

-	Landing Estimate
-	OLTP - Online Transaction Processing
-	OLAP - Online Analytical Processing
-	Out Of Stock & Excess Inventory
-	Query Folding
-	Golden Ratio (1:1.6)

### 🤝 Stakeholder Interaction Insights

-	Usage of Teams Chat
-	Kick Off Meeting: Report Feature & Project Charter
-	Stakeholder Analysis (by scattered chart)
-	Mockups


### ❓ Questions to ask before starting with dashboard

- What is the objective and goals of building this PowerBi dashboard?
- In what terms, the success of this project will be measured?
- What will be time dead-line of the project?
- Do the stakeholders expecting pre-view before the actual release?
- What are all the hopes stakeholders have out of this project?
- what are all fears the stakeholder have in terms of building this dashboard?
- Who all will be using this dashboard and for what purpose?
- What are all expectation the stakeholders have, by the completion of this project?
- What can go wrong while building this project?
- What are all the resources/ data needed to build this dashboard?
- Is there any inputs from stakeholders in terms of design and views of the dashboard?
-How often will the Product owner have meeting with the team.

### ✅ Data Validation
-	Benchmark no. from stakeholder
-	Self-check the Business metrics by calculation
-	UAT – User Acceptance Testing (by main stakeholder)
-	Data Validation in Excel (exported from published Power Bi service)
-	Final stage of validation from each stakeholders


## 🗂️ Data Sources

AtliQ Hardware has provided two SQL databases and four Excel files for analysis.

### Excel Files 
- Operating Expenses – Contains company-wide expense data
- Targets (FY 2022 only) – Sales targets for the fiscal year 2022
- Market Share (Personal Computer Division) – Limited to PC segment analysis
- Country Flag - Contains image of flag of all countries in the world

### SQL Databases 

**Database: gdb041**
**Fact Tables**
- ```fact_forecast_monthly``` – Monthly sales forecasts.
- ```fact_sales_monthly``` – Actual monthly sales data.

**Dimension Tables**

- ```dim_customer``` – Customer details.
- ```dim_market``` – Market segmentation.
- ```dim_product``` – Product information.
- ```dim_country flag``` – image of flag of countries

**Database: gdb056**
**Financial & Cost Data Tables**

- ```freight_cost``` – Logistics and shipping costs.
- ```gross_price``` – Product pricing before discounts.
- ```manufacturing_cost``` – Production expenses.
- ```post_invoice_deductions``` – Discounts applied after invoicing.
- ```pre_invoice_deductions``` – Discounts and adjustments before invoicing.

**Time Frame & Fiscal Year**
AtliQ’s fiscal year runs from September to August.
The dataset includes actual sales data from September 1, 2017, to December 31, 2021.


## ❄️ Data Model

- Data modeling is all about creating relationship between the tables. It plays a vital role and is considered as the basement of report. All the visuals will be built upon the data model.
- Two kinds of table: 
    - Primary table (has unique id) i.e. Dim Table
    - Secondary table (repeated values & transaction) i.e. Fact Table
- In this project, we have followed Snowflakes schema of data modeling because the relationship is not only established with Dim—Fact but also Dim—Dim

  Following Snowfall Data Modeling :

![Data Model](https://github.com/user-attachments/assets/7e105cb3-7c2e-43f7-98e4-66f7361bfb43)


## 🎨 Dashboard Designing

Based on the mockups provided by the main stakeholder, designed the visuals and created measure as and when required

### Home page

In Home page, all the views button will be available. User will land on specific view page by clicking the button 

- Finance View
- Sales View
- Marketing View
- Supply chain View
- Product View
- Executive View
- Information pop-up
- Support pop-up



![home pg](https://github.com/user-attachments/assets/d3d50ab9-36a2-4e39-81cf-7208adb12ffd)




### Finance View

![Finance View](https://github.com/user-attachments/assets/12ecbd0b-35ec-4dc1-9427-f6dcf5e8cd5f)


### Sales View


![Sales View](https://github.com/user-attachments/assets/3a2ee875-f2e3-4365-96a6-f52d27682c33)


### Market View


![Market View](https://github.com/user-attachments/assets/fb4877f2-7fdd-4d69-aec5-c6fc45b8e83e)


### Supply Chain View

![Supply Chain View](https://github.com/user-attachments/assets/4931eded-f79d-4397-b23e-1875e7866f74)


### Product View

![Product View](https://github.com/user-attachments/assets/58322772-af82-46cb-a2e0-5d30edefac6c)


### Executive View


![Executive View](https://github.com/user-attachments/assets/d1b0538b-323b-411d-85da-fa77dae23a67)




  










