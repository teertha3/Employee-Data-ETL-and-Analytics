# Employee Data ETL & Analytics using PySpark

## Project Overview

This project demonstrates an end-to-end employee data ETL workflow using PySpark.

A messy employee dataset was ingested from CSV, validated, cleaned and transformed using PySpark. The processed data was then stored in Parquet format and loaded into Power BI for analysis and visualization.

## Tech Stack

- Python
- PySpark
- Apache Spark
- Parquet
- Power BI
- Google Colab

## Project Workflow

Raw CSV
   ↓
PySpark DataFrame
   ↓
Data Validation
   ↓
Data Cleaning
   ↓
Data Transformation
   ↓
EDA
   ↓
Parquet
   ↓
Power BI
   ↓
Dashboard

## Data Validation
- Checked the number of rows & columns
- Checked the schema
- Checked for null values across columns
- Checked for duplicate records

## Data Cleaning
The following cleaning operations were performed:
- Converted Salary column to double
- Identified and handled invalid salary values
- Imputed missing Age values using the mean
- Imputed missing Salary values using the mean
- Split Department_Region into Department and Region
- Validated the resulting schema

## Transformations & Analysis
The project includes:
- Department-wise employee counts
- Region-wise employee counts
- Average salary by department
- Employee distribution by age
- Performance-score analysis
- Salary ranking within each department using PySpark Window functions

## Data Storage
- After cleaning and transformation, the processed employee data was written to Parquet format using PySpark.
- Parquet was chosen as the final storage format because it is a columnar format well suited for analytical workloads.

## Power BI
- The cleaned Parquet data was loaded into Power BI to create an interactive dashboard for employee analysis.
