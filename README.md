## Credit Card Financial Dashboard (Power BI)



**Project Overview**



This project presents an interactive Credit Card Financial Dashboard built using Power BI, SQL, and DAX. The dashboard provides insights into customer transactions, revenue trends, and credit card performance metrics.



The goal of the project is to help stakeholders monitor and analyze credit card operations through real-time visual analytics and key performance indicators (KPIs)



**Project Objective**



The objective of this project is to develop a comprehensive credit card weekly dashboard that:



Provides real-time insights into credit card transactions



Tracks important business KPIs such as revenue, transaction amount, and interest earned



Monitors customer behavior and card usage trends



Helps stakeholders make data-driven decisions



**Technologies Used**



Power BI – Dashboard visualization



SQL – Data storage and data extraction



DAX (Data Analysis Expressions) – Calculations and measures



CSV Dataset – Source data for analysis



**Project Workflow**



1. Data Collection



The dataset is imported from CSV files and stored in a SQL database.



Steps:



Prepare the CSV data files



Create tables in SQL database



Import CSV files into SQL tables



2. Data Processing



Data is cleaned and transformed before visualization.



Key operations:



Data modeling



Data transformation



Relationship building between tables



3. DAX Calculations



Several calculated columns and measures are created using DAX.



Examples:



Age Group Classification



AgeGroup = SWITCH(

&#x20;TRUE(),

&#x20;'public cust\_detail'\[customer\_age] < 30, "20-30",

&#x20;'public cust\_detail'\[customer\_age] >= 30 \&\& 'public cust\_detail'\[customer\_age] < 40, "30-40",

&#x20;'public cust\_detail'\[customer\_age] >= 40 \&\& 'public cust\_detail'\[customer\_age] < 50, "40-50",

&#x20;'public cust\_detail'\[customer\_age] >= 50 \&\& 'public cust\_detail'\[customer\_age] < 60, "50-60",

&#x20;'public cust\_detail'\[customer\_age] >= 60, "60+",

"Unknown"

)



**Revenue Calculation**



Revenue =

'public cc\_detail'\[annual\_fees] +

'public cc\_detail'\[total\_trans\_amt] +

'public cc\_detail'\[interest\_earned]





**Dashboard Insights**



1. Key insights from the dashboard include:



2. Revenue increased 28.8% week-over-week



3. Total transaction amount and count increased



4. Customer count increased



5. Overall yearly revenue reached 57M



6. Total interest earned 8M



7. Total transaction amount 46M



8. Male customers contribute 31M revenue, female 26M



9. Blue & Silver credit cards contribute to 93% of transactions



10. Texas, New York, and California contribute 68% of revenue



11. Overall activation rate: 57.5%



12. Overall delinquent rate: 6.06%



**Dashboard Features**



1. Weekly revenue tracking



2. Customer segmentation



3. Card category analysis



4. Transaction monitoring



5. Geographic revenue distribution



6. Activation and delinquency metrics



**Project Structure**



Credit\_Card\_Financial\_Dashboard

│

├── dataset

│   ├── customer\_data.csv

│   └── transaction\_data.csv

│

├── SQL

│   └── data\_import\_queries.sql

│

├── PowerBI

│   └── credit\_card\_dashboard.pbix

│

└── README.md



**How to Run the Project**



1. Download the dataset.



2. Import CSV files into SQL database.



3. Run SQL queries to prepare tables.



4. Open the Power BI (.pbix) file.



5. Connect Power BI to the SQL database.



6. Refresh data to view the dashboard.



**Dashboard Preview**
![project](https://github.com/suryansh-johri/Credit-Card-Financial-Dashboard-/blob/main/image1.png)
![project](https://github.com/suryansh-johri/Credit-Card-Financial-Dashboard-/blob/main/image2.png)







**Author**\
**Suryansh Johri**

