# customer_behavior_analysis
Data analytics project showcasing customer behavior analysis using Python, SQL and Power Bi.

📊 Data Analytics Project

📌 Overview

This project demonstrates an end-to-end data analytics workflow, starting from raw dataset exploration and cleaning to SQL analysis and interactive dashboard creation.

The project uses Python and Jupyter Notebook for data exploration and preprocessing, MySQL for querying and analysis, and Power BI for creating an interactive dashboard. A final project report was also created, along with a presentation prepared using Gamma AI.

The goal of the project is to transform raw data into meaningful insights that can support data-driven decision-making.

📂 Dataset

The project begins with a raw dataset that is loaded and analyzed using Python.

The dataset was examined to understand:

Dataset structure and dimensions
Data types
Missing values
Duplicate records
Outliers and inconsistencies
Key numerical and categorical variables
Relationships and patterns within the data

Dataset: customer_shopping_behavior.csv

🛠️ Tools & Technologies
Tool	Purpose
Python	Data analysis and preprocessing
Jupyter Notebook	EDA and data cleaning
Pandas	Data manipulation
MySQL	SQL-based data analysis
Power BI	Interactive dashboard
Gamma AI	Project presentation
GitHub	Project documentation and version control

🔄 Project Workflow
Raw Dataset
     ↓
Data Loading
     ↓
Exploratory Data Analysis (EDA)
     ↓
Data Cleaning & Preprocessing
     ↓
Clean Dataset
     ↓
MySQL Data Analysis
     ↓
SQL Queries & Insights
     ↓
Power BI Dashboard
     ↓
Report & Presentation

🐍 Step 1: Load Dataset in Python

The dataset was imported into a Jupyter Notebook using Pandas.

Initial analysis was performed to understand the structure and quality of the data.

Example:

import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")

df.head()
df.info()
df.shape
df.describe()

🔍 Step 2: Exploratory Data Analysis

Exploratory Data Analysis was performed to identify important patterns, trends, and potential data quality issues.

The analysis included:

Understanding numerical and categorical variables
Checking distributions
Identifying missing values
Detecting duplicate records
Analyzing outliers
Studying relationships between variables


🧹 Step 3: Data Cleaning

After completing the initial analysis, the dataset was cleaned and prepared for further analysis.

Key cleaning activities included:

Handling missing values
Removing duplicate records
Correcting data types
Standardizing inconsistent values
Treating outliers where appropriate
Renaming columns for better readability
Preparing the final dataset for SQL analysis

The cleaned dataset was then exported for use in MySQL.

🗄️ Step 4: MySQL Analysis

The cleaned dataset was imported into MySQL to perform structured data analysis using SQL.

SQL queries were written to answer business-related questions and identify useful insights.

The analysis included concepts such as:

SELECT
WHERE
GROUP BY
ORDER BY
Aggregate functions
CASE WHEN
Subqueries
Common Table Expressions (CTEs)
Window functions, where applicable

Example:

select item_purchased, round(avg(review_rating),2)
 as "Average Product Rating" 
from customertable
group by item_purchased
order by avg(review_rating) desc
limit 5;

The SQL analysis helped identify key trends and metrics that were later incorporated into the Power BI dashboard.

📊 Step 5: Power BI Dashboard

The cleaned and analyzed data was used to create an interactive Power BI dashboard.

The dashboard was designed to provide a clear overview of the most important findings.

Dashboard Features
Interactive charts
Category-wise analysis
Trend analysis
Filters and slicers
Comparative analysis
Summary of key business metrics

The dashboard allows users to interact with the data and explore different aspects of the analysis.


📈 Results & Key Insights

The analysis produced several insights from the dataset, including:

Identification of important trends and patterns
Comparison of different categories and segments
Identification of high- and low-performing areas
Analysis of key business metrics
Detection of data quality issues
Identification of factors contributing to overall performance

The final Power BI dashboard presents these insights in an easy-to-understand visual format.


📝 Project Report

A detailed project report was prepared to document the complete analytical process.

The report covers:

Project objective
Dataset description
Data exploration
Data cleaning
SQL analysis
Power BI dashboard
Key findings
Business insights
Conclusion

🎤 Presentation

A PowerPoint presentation was created to summarize the project, methodology, dashboard, and key findings.

Gamma AI was used to assist in creating and designing the presentation.

The presentation provides a concise overview of the project and its results.

▶️ How to Run the Project
1. Clone the Repository using the git clone command.

2. Install Python Libraries
pip install pandas numpy jupyter

3. Open the Jupyter Notebook
jupyter notebook

Open the project notebook and run the cells sequentially.

4. Set Up MySQL
Install MySQL.
Create a database.
Import the cleaned dataset.
Run the SQL queries provided in the SQL folder.

Example:

CREATE DATABASE analytics_project;

USE analytics_project;

5. Open the Power BI Dashboard

Open the .pbix file using Power BI Desktop.

If required, update the data source connection to point to your local MySQL database.

📁 Project Structure

data-analytics-project/
│
├── data/
│   ├── raw/
│   │   └── dataset.csv
│   └── cleaned/
│       └── cleaned_dataset.csv
│
├── notebooks/
│   └── EDA_Data_Cleaning.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── analytics_dashboard.pbix
│
├── report/
│   └── project_report.pdf
│
├── presentation/
│   └── project_presentation.pptx
│
├── images/
│   └── dashboard.png
│
└── README.md

🎯 Skills Demonstrated

This project demonstrates practical experience in:

Data Cleaning & Preprocessing
Exploratory Data Analysis
Python & Pandas
SQL & MySQL
Data Visualization
Power BI Dashboard Development
Business Intelligence
Data Storytelling
Report Writing
Presentation Development
🚀 Conclusion

This project demonstrates a complete end-to-end data analytics workflow, from raw data to actionable insights.

By combining Python, SQL, and Power BI, the project shows how data can be cleaned, analyzed, visualized, and communicated effectively to support business decision-making.

Feel free to explore the repository and review the notebook, SQL queries, dashboard, report, and presentation.
