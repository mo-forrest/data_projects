## Superstore Analysis

The fifth project I worked on during TripleTen’s Business Intelligence Analytics program was a project to identify what caused the high number of returns at the Superstore. Prepare an analysis to understand what caused customers to return their orders and recommend strategies to reduce the volume of returns.

![image](https://github.com/user-attachments/assets/404487b8-256b-40d9-916e-3ab1da12de21)


## Table of Contents for Repository
| File Number | Title | Description |
|:-----------:| ------| ----------- |
| 1 | Superstore Analysis PDF | Completed project in a downloadable format. |
| 2 | Superstore Analysis in Tableau | Completed project in Tableau. |
| 3 | README.md | This page with all the relevant information for the project. |
| 4 | Superstore Analysis Dashboard | Dashboard of sheets analyzing return rates. |
| 5 | Superstore Dashboard Mockup | Mockup to visualize the dashboard. |
| 6 | Superstore Story Arc | Story Arc about the dashboard. |
| 7 | Requirements.txt | A simple text file with all the project requirements provided by TripleTen. |
| 8 | Storytelling with Data Rubric | Criteria for the project. |
| 9 | Reviewer Grade | Comments from the reviewer. |

## Table of Contents for the README.md
| Section Title | Description |
| :------------: | ----------- |
| Description | Describes the project’s purpose, software, format and included visuals. |
| Process | General outline of project from start to finish. |
| Data | Data source, including files, tables, and fields. |
| Assumptions | Assumptions made based on the data and Tripleten. |
| Findings | Insights learned from the data analysis. |
| Recommendations | Recommend next steps for business stakeholders. |

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

## Recommendations
