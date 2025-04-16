## Superstore Analysis

The fifth project I worked on during TripleTen’s Business Intelligence Analytics program was a project to identify what caused the high number of returns at the Superstore. Prepare an analysis to understand what caused customers to return their orders and recommend strategies to reduce the volume of returns.

![image](https://github.com/user-attachments/assets/404487b8-256b-40d9-916e-3ab1da12de21)


## Table of Contents for Repository
| File Number | Title | Description |
|:-----------:| ------| ----------- |
| 1 | [Superstore Analysis PDF](https://github.com/mo-forrest/data_projects/blob/471019d4959356c1c6839e7686788dc3f8bdd7da/Superstore/Superstore%20Analysis%20PDF.pdf) | Completed project in a downloadable format. |
| 2 | [Superstore Analysis in Tableau](https://github.com/mo-forrest/data_projects/blob/c7fe68311b90bce685335176d7ef84a1d70cb35b/Superstore/Sprint%205%20Project%20Final.twbx) | Completed project in Tableau. |
| 3 | README.md | This page with all the relevant information for the project. |
| 4 | [Superstore Analysis Dashboard](https://github.com/mo-forrest/data_projects/blob/c7fe68311b90bce685335176d7ef84a1d70cb35b/Superstore/Superstore%20Dashboard.png) | Dashboard of sheets analyzing return rates. |
| 5 | [Superstore Dashboard Mockup](https://github.com/mo-forrest/data_projects/blob/c7fe68311b90bce685335176d7ef84a1d70cb35b/Superstore/Superstore%20Mockup.png) | Mockup to visualize the dashboard. |
| 6 | [Superstore Story Arc](https://github.com/mo-forrest/data_projects/blob/26c2f3e1a49bb11ac099c853788edf6ea8468885/Superstore/Story%20Arc%20Photo.png) | Story Arc about the dashboard. 
| 7 | [Storytelling with Data Rubric](https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/remodeled/files/Storytelling_with_Data_Rubric.pdf) |Criteria for the project with all requirements provided by TripleTen. |
| 8 | [Reviewer Feedback](https://github.com/mo-forrest/data_projects/blob/37990d3b02c345dd11e4fb287506a2054b9405d1/Superstore/Reviewer%20Feedback.docx) | Comments from the reviewer. |


## Table of Contents for README.md
| Section Title | Description |
| :------------: | ----------- |
| [Description](https://github.com/mo-forrest/data_projects/blob/main/Superstore/README.md#description) | Describes the project’s purpose, software, format and included visuals. |
| [Process](https://github.com/mo-forrest/data_projects/blob/main/Superstore/README.md#process) | General outline of project from start to finish. |
| [Data](https://github.com/mo-forrest/data_projects/blob/main/Superstore/README.md#data) | Data source, including files, tables, and fields. |
| [Assumptions](https://github.com/mo-forrest/data_projects/blob/main/Superstore/README.md#assumptions) | Assumptions made based on the data and Tripleten. |
| [Findings](https://github.com/mo-forrest/data_projects/blob/main/Superstore/README.md#findings) | Insights learned from the data analysis. |
| [Recommendations](https://github.com/mo-forrest/data_projects/blob/main/Superstore/README.md#recommendations) | Recommend next steps for business stakeholders. |

## Description
* 9 worksheets in Tableau and Excel
* Includes data analysis, dashboard, mock up and story arc.

## Process
First, I cleaned the data and I focused on the root cause of returns. I left joined the Returns table to the Orders table, and used a calculated field where the null values were 0 and the Yes values were 1. Next I created worksheets to analyze different views on return rates.

* Scatterplot showing the correlation between total sales and total returns, aggregated it by product subcategory.
* Bar chart showing the return rate by product category.
* Horizontal bar chart of the return rate by customer, including filters to filter out the null values and count the number of returns per customer.
* Symbol map of the return rate by state to show any differences in returns by region.
* Line chart of the return rate by month and category to determine if there are seasonal influences on returns.
* Line chart of return rate by state and category to show the return rate for a mix of multiple factors


Then I made a dashboard to showcase the analysis. I used a mockup to plan the layout, and a story arc to highlight key points in the presentation.


## Data
* 'Superstore.xls': raw transaction logs
  * 'Row ID': unique identifier for customers
  * 'Order ID': ID number for orders
  * 'Order Date': date of the order
  * 'Ship Date': date the order shipped
  * 'Shipe Mode': mode of shipping
  * 'Customer ID': ID name for customers
  * 'Customer Name': name of the customer on the order
  * 'Segment': group category for the customer
  * 'Country/Region': country or region of the customer and order
  * 'City': city the order was placed
  * 'State': state the order was placed
  * 'Postal Code': postal code of the order
  * 'Region': region the order was placed
  * 'Product ID': ID of the product in the order
  * 'Category': category of the order
  * 'Sub-Category': sub-category of the order
  * 'Product Name': product name of the order


## Assumptions
* All data in the Superstore excel sheet are correct.


## Findings
* Technology is the category most returned.
* Root cause of returns are customers making high returns between 2-14 items each.
* California, New York and Washington make the highest returns by region.
* Returns spike twice a year in September and December.
  

## Recommendations
* **Technology is the category most returned:** To reduce returns the Superstore can prioritize selling warranties for products and limit the timeframe to make returns in this category. Promotions can also be offered to customers to make exchanges or receive store credit.
* **Root cause of returns are customers making high returns between 2-14 items each:** To reduce returns, returns for customers can be limited per year and customers who make more than 5 returns per year can be flagged and monitored for suspicious activity. 
* **California, New York and Washington make the highest returns by region:** To reduce returns, the company can prioritize implementing the return strategies listed above in these locations first. Including prioritizing warranties, limiting timeframes for returns, offering promotions to make exchanges or receive store credit and monitoring customers who make a high number of returns.
* **Returns spike twice a year in September and December:** To reduce returns, the Superstore can prioritize promotions and the marketing budget during these months.
