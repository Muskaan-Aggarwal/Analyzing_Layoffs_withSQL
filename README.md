# Analyzing Layoff Data SQL Project
 **This project analyzes global layoff data using SQL for data cleaning and exploratory data analysis (EDA).**
 
 **The dataset is sourced from Kaggle: Layoffs 2022.**

## Project Structure
- **data_cleaning.sql**: SQL scripts for cleaning and preparing the layoff data.
- **EDA.sql**: SQL queries for exploratory data analysis on the cleaned dataset.

## Workflow
**1. Data Cleaning (data_cleaning.sql)**
- Create staging tables: Copies raw data into a staging table for processing.
- Remove duplicates: Identifies and deletes duplicate records using ROW_NUMBER().
- Standardize data: Cleans up inconsistencies in columns such as industry and country.
- Fix date formats: Converts date strings to SQL DATE type.
- Handle nulls: Fills missing values where possible and removes rows with insufficient data.
- Optimization: Remove any columns and rows that are not necessary - few ways
  
**2. Exploratory Data Analysis (EDA.sql)**
- Summary statistics: Find max/min layoffs and analyze layoff percentages.
- Company analysis: Identifies companies with the largest layoffs (single and total).
- Location and Industry Trends: Aggregate layoffs by location, country, industry, and stage.
- Time series: Examines layoffs by year and computes rolling totals by month.
- Ranking: Uses window functions to rank companies by layoffs per year.
  
## How to Use
- Import the dataset into your SQL database as world_layoffs.layoffs.
- Run data_cleaning.sql to clean and prepare the data.
- Run EDA.sql to perform exploratory analysis and generate insights.

## Requirements
- MySQL or compatible SQL database (window functions and CTEs required)
- Access to the Kaggle layoff dataset (Layoffs 2022)
