## Shopify Analysis

For my sixth project in Tripleten’s Business Intelligence Analytics program, I reviewed the landscape of apps on the Shopify platform using data scraped from public Shopify websites. The purpose of the project was to identify key factors that play into the success of a Shopify app. Results were shared in a Power BI report.

![image](https://github.com/user-attachments/assets/50826d31-7d96-4163-b9fc-cd3feda6dc28)


## Table of Contents for Repository Artifacts

| File Number | Title | Description |
| :-----------: | ----- | ----------
| 1 | [Shopify Analysis PDF](https://github.com/mo-forrest/data_projects/blob/eaf19b1dc4b6b3c4ebb749999ad7c63090e71fad/Shopify/Shopify%20Analysis%20PDF.pdf) | Completed project in a downloadable pdf. |
| 2 | README.md | This page with all relevant information to the project. |
| 3 | [App Landscape Sheet](https://github.com/mo-forrest/data_projects/blob/5352c2e24f45c868a6ed8c7c8d1d2366180d74e4/Shopify/App%20Landscape%20Screenshot.png) | Key statistics on the types of apps that are out there. |
| 4 | [Reviews Screenshot](https://github.com/mo-forrest/data_projects/blob/5352c2e24f45c868a6ed8c7c8d1d2366180d74e4/Shopify/Reviews%20Screenshot.png) | Reviews rated by how helpful the developers were found. |
| 5 | [App Reviews](https://github.com/mo-forrest/data_projects/blob/5352c2e24f45c868a6ed8c7c8d1d2366180d74e4/Shopify/App%20Reviews%20Screenshot.png) | Developers rated by most responsive to least responsive. |
| 6 | [Requirements](https://github.com/mo-forrest/data_projects/blob/a0a8f04c8abacc7ea303b0299f679d139cc18d74/Shopify/Requirements.docx) | Criteria for project submission. |
| 7 | [Reviewer Commments](https://github.com/mo-forrest/data_projects/blob/69c7b7977470cc4f3fd5b58f805266d6ba578b39/Shopify/Reviewer%20Feedback.docx) | Comments from the reviewer. |


## Table of Contents for README.md

| Section Title | Description |
| :------------:| ------------ |
| [Description](https://github.com/mo-forrest/data_projects/tree/main/Shopify#description) | Describes the project’s purpose, software, format and included visuals.|
| [Process](https://github.com/mo-forrest/data_projects/tree/main/Shopify#process) | General outline of project from start to finish. |
| [Data](https://github.com/mo-forrest/data_projects/tree/main/Shopify#data) | Data source, including files, tables, and fields. |
| [Assumptions](https://github.com/mo-forrest/data_projects/tree/main/Shopify#assumptions) | Assumptions made based on the data and Tripleten. |
| [Findings](https://github.com/mo-forrest/data_projects/tree/main/Shopify#findings) | Insights learned from the data analysis. |
| [Reccommendations](https://github.com/mo-forrest/data_projects/tree/main/Shopify#recommendations) | Recommend next steps for business stakeholders.|


## Description
* 4 worksheets in Power BI and Excel
* Includes data analysis and data source


## Process
First I cleaned the data. Then I started working on the App Landscape sheet to identify key statistics on the types of apps on the Shopify platform. On the App Landscape sheet I created a:
* KPI card that counts the unique number of apps.
* Line Chart to get the sum of the review count and last modified date.
* Scatterplot of review count and average rating.
* Scatterplot with the reviews_count on the X axis and the average rating.

Next, I made a Reviews sheet to rate reviews by how helpful developers have been to customers. On the Reviews sheet I created a:
* New column in the Reviews table using a DAX expression that multiplied the rating by 1+helpful_count and a card with the average value of the new helpful_reviews column.
* New column in the Reviews table using a DAX expression named developer_answered which identified 1 for True and 0 for False if the row is blank. I used this new column to create a scatterplot comparing the average rating by the value of the developer_answered column.

Finally, I made an App Reviews sheet to rate developers by most responsive to least responsive. To do this, I would have:
* Created a new relationship between the Reviews table and the Apps table in the data model. With  the app_id column from the Reviews table and the id column from the Apps table, I made the relationship many-to-one to make a bar chart with the developer and the sum of rating.
* To reduce any confusion, because an app could have a high sum of rating due to many one-star reviews, I made a new bar chart with developer against the helpful_review average.
* Created a bar chart with the developer from the apps table and the developer_answered column to identify which developers were most responsive. I added a filter for this visual that selects only the rows where reviews_count is greater than 500.

  
## Data
The shopify.xlsx dataset contains public data scraped from the Shopify App Store. It includes 4 tables:
- **apps**: Details of the apps on Shopify apps marketplace.
- **apps_categories**: Join tables to connect apps with categories.
- **categories**: Categories of the apps. Each app has multiple categories.
- **reviews**: Each review (row) contains information on user opinion about the related app (rating and comment). Also, any responses from the developers.

## Assumptions
* All data scraped from the Shopify App Store is reliable and accurate.
  
## Findings
* Developers who answered more questions had higher ratings.
* Average rating of helpful reviews is 5.48.
* Developers who answered more questions were viewed as more helpful than other developers.

## Recommendations 
* **Developers who answered more questions had higher ratings:** Shopify apps with developers who answer questions boost the rating of the app on the platform. Shopify apps can create policies that require developers to engage with others to keep their ranking on the Shopify platform.
* **Average rating of helpful reviews is 5.48:** Shopify apps should create incentives for developers to score helpful reviews and reward employees who make an impact on the business.
* **Developers who answered more questions were viewed as more helpful than other developers:** By implementing a requirements and reward system, Shopify Apps will continue to see helpful reviews for developers which will enforce the behavior and maintain these stats over time.


