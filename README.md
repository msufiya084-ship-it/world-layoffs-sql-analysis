# World Layoffs: Data Cleaning and EDA in SQL

## Project Overview
This project focuses on cleaning and analyzing a global dataset of company layoffs (2020–2023) using MySQL. 

The main goals were to take a raw dataset with inconsistent formatting, duplicate entries, and missing fields, clean it up systematically, and run exploratory queries to identify key trends across industries, locations, and time periods.

## Key SQL Techniques Used
Data Deduplication: Using CTEs and `ROW_NUMBER()` partitioned across multiple fields to flag and delete duplicate records.
Data Standardization: Cleaning whitespace (`TRIM()`), unifying inconsistent industry labels (e.g., standardizing crypto-related terms), and cleaning country names.
Type Conversion & Date Formatting: Converting text-formatted date strings into SQL `DATE` format using `STR_TO_DATE()` and altering table schemas.
Handling Nulls: Using self-joins to populate missing industry values based on matching company/location data.
Advanced Aggregations & Window Functions: Utilizing `SUM()`, `MAX()`, `DENSE_RANK()`, and rolling total calculations to rank top companies by workforce reduction per year.

## Repository Contents
`world_layoffs_project.sql` - Full SQL script containing both data cleaning steps and exploratory analytical queries.

