# SalesVision


## Overview
This project aims to provide sales insights for Atliq Hardware using Microsoft Power BI for data cleansing and visualization. Additionally, MySQL is utilized as the database to analyze the data effectively.

## Key Metrics and Queries
- Total Transaction: To find out the total transactions of the company, use the following code in Microsoft Power BI:
Total Transaction = COUNTROWS('sales transactions')

- Revenue: To calculate the revenue of the company, use the following code in Microsoft Power BI:
Revenue = SUM('sales transactions'[sales_amount])

- Revenue in SQL (2020): To see the revenue of the company in SQL for the year 2020, execute the following SQL query:
SELECT SUM(sales_amount)
FROM transactions AS trns
INNER JOIN date AS dt ON trns.order_date = dt.date
WHERE dt.year = 2020


- Distinctive Years in SQL: To view the distinctive years in SQL, use the following query:
SELECT DISTINCT(year) FROM date


## Instructions
Copy and paste the provided queries and code snippets into your Microsoft Power BI or SQL environment to analyze sales data effectively.

## Additional Notes
- Ensure that the appropriate data sources are connected to your Power BI and MySQL environments for accurate analysis.
- Customize the queries and calculations based on specific requirements and business objectives.


## License
This project is licensed under the [MIT License](LICENSE).


![Screenshot 2024-02-17 110410](https://github.com/yppaarth/Sales_insight_Bi/assets/78694506/5b25cd81-d1fd-4c0f-9fcd-0ae229bfd8b4)



