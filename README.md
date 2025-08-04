# ACE Superstore Sales Dashboard – Excel Project


## Introduction
In this project, I developed an interactive sales dashboard to identify regional performance gaps, customer behaviour patterns, and product category profitability. The dashboard provides a comprehensive view of sales data, enabling the executive team to focus on high-impact areas in subsequent strategy sessions.

I was given two datasets: ACE Superstore Retail Dataset which contained 1 table and the Store Locations dataset which also contained 1 table. I copy and pasted the Store Locations table into a blank sheet in the ACE Superstore Retail Dataset spreadsheet so I was only working in one spreadsheet with one dataset. 


## About the Dataset
The dataset contains information from ACE, a nationwide retail chain, structured into two tables:
- in – Contains details of customer purchases, including quantity, sales, cost, and date.
- Store Locations – Contains details of ACE store, including City, Postal Code, Country and Region.


## Problem Statement
ACE has seen significant sales growth over the past two years. As the company prepares to expand into additional regions and optimize its current operations, senior leadership requires an introductory business intelligence report summarizing key sales performance trends.
My role as a newly onboarded data analyst is to perform an initial data exploration and create a report that answers foundational business questions using the sales dataset.


## My Approach and Tools Used
To create this dashboard I used Excel, ensuring accuracy and interactivity.


### Data Cleaning

#### 1. Remove duplicates: 
- Firstly, I checked for duplicates in both tables using the remove duplicates tool in the data tab. No duplicates were found

#### 2. Correct typing errors: 
- I found and corrected data entry errors in both tables. For example, 'Yorkshire & the Humber' and 'Yorkshire and the Humber' also in Category column - 'Food: Oil' and 'Food: Oils' etc

#### 3. Blank values: 
- None in Store Locations table but the 'in' table had 4 columns with blanks: discount, category, region and country. The discount column blanks were set as 0, the region and country blanks were corrected using the Store Locations table (XLOOKUP) and the category blanks were filled using subcategory column.

#### 4. Concise wording for category column in 'in' table: 
- Assigned same name for like items, for example Bakery and Bakery Goods etc

#### 5. Create columns ready for analysis: 
- Added columns to the 'in' table such as Segment, Revenue, COS, Profit and Red Flags. The red flag column was added as some costs had negative figures which after investigating with the team, I determined as an error, and will be using this column to filter out these anomalies when analysing the data


### Data Analysis

#### 1. Pivot Tables: 
- Created 7 pivot tables from the 'in' table

#### 2. Calculated field: 
- To calculate the margin in one of the pivot tables, I created the calculated field Profit Margin (Profit/Revenue)

#### 3. Graphs: 
- Created graphs for dashboard using the pivot tables. I then used the chart design settings to customise the graph
  
### Final Dashboard
![Aamina_Patel_Dashboard](https://github.com/user-attachments/assets/cabdcc48-afd2-47ad-9c49-a3fcebec6e45)

## Insights from the Dashboard
The dashboard provides a comprehensive breakdown of sales, revenue, and regional performance. Key insights include:

#### 1. Order & Revenue Trends
- Total orders: 10,958
- Revenue: £2,687,850.46
- COS: £1,044,119.84
- Gross Profit: £1,643,730.62
Highest revenue was generated in 2024 and currently 2025 is underperforming compared to 2024.
  
#### 2. Location-Based Profitability
- Top-performing location: East Midlands generated the most profit at £268,446.22
- Low-performing location: North East generated the least profit at £18,373.75

#### 3. Online vs Instore
- 51% of revenue came from online orders showing a minor preference for online shopping

#### 4. Revenue per Product
- Top-performing products: Portable Solar Generator, Portable Refrigerator Freezer, Electric Bike, Digital Camera, Compact Dishwasher (High to Low)
- Low-performing products: Cinnamon Raisin Bagels, Baking Soda, Canned Black Beans, Paprika, Instant Mashed Potatoes (Low to High)


## Conclusion & Recommendations

#### Key Takeaways
- Revenue in 2025 is lower than 2024
- East Midlands is the region with the highest profitability and North East has the lowest
- There is a slight preference towards online shopping
- Revenue per product shows us that customers prefer our electronic items over food items

#### Recommendations
- To increase revenue ACE could launch a loyalty programme
- Expand stores in regions with high profitability
- To boost online sales we could sell our high performing items at a discount on the ACE website
- Increase our inventory of high performing products and try to phase out low performing products

### Realcare Tech Mark Data Analyst Mentorship Programme
- Created by: Aamina Patel
- Built with: Microsoft Excel (Pivot Tables)
- Data Source: RealCare Tech Mark LTD
