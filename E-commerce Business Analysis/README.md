## E-commerce Business Analysis

The third project I worked on during Tripleten's Business Intelligence Analytics program was an assignment to analyze the raw transaction logs of an E-commerce company. These transactions included activities and events by users on the company’s website like viewing a product page, opening their shopping cart, or completing a purchase. The purpose of this assignment was to analyze the company’s raw transaction logs and turn these event logs into business metrics.

![image](https://github.com/user-attachments/assets/275db780-df08-4afa-a20d-525619cc7adb)


Google Spreadsheet can be found [here](https://github.com/mo-forrest/data_projects/blob/c89fbe9738e72579d1315f835f423632d0e82644/E-commerce%20Business%20Analysis/Ecommerce%20Business%20Analysis.xlsx). Raw data Google Spreadsheet can be found [here](https://github.com/mo-forrest/data_projects/blob/9b6488c3dca9a5655f8971f2cfa1b2b5164fcabb/E-commerce%20Business%20Analysis/Raw%20User%20Activity.xlsx).



## Table of Contents for Repository Artifacts

| File Number | Title | Description |
| :-----------: | ----------- |----------- |
| 1 | [E-commerce Business Analysis PDF](https://github.com/mo-forrest/data_projects/blob/fad597cc853f72a3fed695c9f58a9465fea13f75/E-commerce%20Business%20Analysis/E-Commerce%20Business%20Analysis.pdf) | The completed project in a downloadable pdf file. |
| 2 | README.md | This page with all relevant information to the project. |
| 3 | [Requirements.txt](https://github.com/mo-forrest/data_projects/blob/d070a7ed084d16fa75926accc2e35add59b66c2f/E-commerce%20Business%20Analysis/Requirements.txt) | Project requirements as defined by TripleTen. |
| 4 | [ReviewerGrade.png](https://github.com/mo-forrest/data_projects/blob/a30ba41527f59beb2b804b6573f0565389c8ba0e/E-commerce%20Business%20Analysis/Reviewer%20Feedback.png) | Project feedback from reviewer.|



## Table of Contents for README.md

| Section Title | Description |
| :------------: | ----------- | 
| [Description](https://github.com/mo-forrest/data_projects/blob/main/E-commerce%20Business%20Analysis/README.md#description) | Describes the final product's purpose, software, format, and included visuals. |
| [Process](https://github.com/mo-forrest/data_projects/blob/main/E-commerce%20Business%20Analysis/README.md#process) | Outline of how this project was created from start to finish. |
| [Data](https://github.com/mo-forrest/data_projects/blob/main/E-commerce%20Business%20Analysis/README.md#data) | Describes the source of data, including files, tables, and fields. |
| [Assumptions](https://github.com/mo-forrest/data_projects/blob/main/E-commerce%20Business%20Analysis/README.md#assumptions) | Describes assumptions to include from TripleTen and assumptions made based on the data and task. |
| Findings | Insights learned from the data analysis. |
| Recommendations | Recommedations for the stakeholders based on the analysis. |


## Description:
* 8 page spreadsheet
* Includes raw data, processed data, data analysis, and pivot tables.


## Process:
I first explored, filtered, and cleaned the data. Then I created and built a conversion funnel. I prepared data for cohort analysis. Calculated retention rates. Lastly, I finalized the formatting and documentation for the client's readability.


## Data:
The data was one Google spreadsheet provided by TripleTen. Raw data Google Spreadsheet can be found [here](https://github.com/mo-forrest/data_projects/blob/9b6488c3dca9a5655f8971f2cfa1b2b5164fcabb/E-commerce%20Business%20Analysis/Raw%20User%20Activity.xlsx).

* 'Business Analyst Project.csv': raw transaction logs
  * 'raw_user_activity': Each row represents an activity, or event, by a user on the company’s website
    * 'user_id': unique customer IDs
    * 'event_type': the type of activity by the user
    * 'category_code': category of the product being viewed or purchased
    * 'brand': the company that makes the product
    * 'price': price of the product, in USD
    * 'event_date': date of the user activity, in YYYY-MM-DD format
  * 'Table of Contents': Preformated yet empty table of contents sheet
  * 'Executive Summary: Preformated yet empty executive summary sheet

## Assumptions:
  * The "raw_user_activity" sheet accurately reflects all website activity for the relevant timeframe.
  * Missing values or inconsistencies in the data are minimal and can be ignored.
  * The provided data format (columns, data types) is correct and consistent.


## Findings:
| Results | Synopsis |
| :------------: | ----------- | 
| Conversion Funnel | The total conversion rate stands at 82%, with shoppers who viewed items, added them to their cart, and completed a purchase. Specifically, 29% of users added items to their cart after viewing them, and 36% of those users went on to purchase the items in their cart.|
| Retention Rates | There was a decline in users between months 1 and 2, but user numbers have steadily increased from months 3 to 4. |


## Recommendations
* Address Shopping Cart Abandonment and Purchase Conversion. Future projects can focus on the best approach such as product page vs checkout process as a source of funnel deterioration.
* Enhance customer engagement and loyalty. Potential marketing campaigns could be personalized communications, loyalty programs, and looking into customer support.
* Gain customer feedback for a more targeted strategy.
* Continue data-driven insights to follow changes in the cohort analysis.

