# DSA2040A Load Phase –  INGABIRE Catherine -671041

## Objective
This project demonstrates the Load stage of the ETL (Extract, Transform, Load) pipeline for the DSA 2040A course.  
It focuses on saving the transformed datasets into different formats, verifying data integrity, and preparing the project for GitHub submission.

---

## Load Phase Overview
In this stage, previously transformed datasets (`transformed_full.csv` and `transformed_incremental.csv`) were loaded into two formats:

1. SQLite database using the `sqlite3` library  
2. Parquet format using the `pandas.to_parquet()` method

---

## Process Summary

### Step 1: Load Transformed Data
The transformed datasets were read from the previous ETL project using:
```python
pd.read_csv('path/to/transformed_full.csv', encoding="ISO-8859-1")
