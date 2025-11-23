# JobStreet Indonesia 2024 — Salary & Job Market Analysis
This repository contains a full exploratory data analysis (EDA) of 32,976 job postings from JobStreet Indonesia (2024).
The project focuses on understanding salary distribution, job market trends, and location-based insights across Indonesia.
data source: https://www.kaggle.com/datasets/husnind/indonesia-average-job-salary?select=job_salary_mean.csv 

# Key Analyses 
1. Location-Based Analysis : cities with the highest salary ranges, which regions offer the most job opportunities,
   salary gap between Jakarta vs non-Jakarta cities
<details>
  <summary>Click to view SQL Query</summary>
--cities with the highest salary ranges
```select 
	location,
	round(avg(salary),2) as avg
from id_jobs 
group by location
order by avg desc 
limit 10
```

</details>

3. 
4. Company-Level Analysis : companies with the most job postings, companies offering above-average salaries
5. Job Demand Trends : top 20 most common job titles, categories with rising or declining demand
   
# Visualizations 
   

# Data Validation 
-No missing values detected, dataset is fully complete

# Skills Used in This Analysis 
1. SQL : to clean, filter, and explore the dataset using SQL. 
Core Querying : - select, where, order by, group by, having 
                - filtering salary ranges 
                - sorting highest-paying jobs 
                - grouping by location or company 
String Operations : - ilike/like for text matching 
                    - lower() /upper()
                    - trim(), replace()
Aggregations 
Joins 
CTE 
Window Functions : row_number(), rank(), dense_rank(), over(partition by..)

2. Power BI : data modeling, DAX, dashboard, map visualization, filter by job title, company, or salary range

# General Data Analyst Skills 
- Feature interpretation
- Insight storytelling
- Documentation

   


