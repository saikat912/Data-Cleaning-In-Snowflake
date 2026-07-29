# 🧹 Data Cleaning in Snowflake: Techniques to Clean Messy Data

A hands-on Snowflake SQL project demonstrating practical data cleaning and transformation techniques commonly used by Data Analysts and Data Engineers. This project walks through cleaning messy customer data, standardizing formats, handling duplicates, and preparing datasets for analytical use. 

---

## 📖 Project Overview

Real-world datasets are rarely clean. This project simulates a marketing scenario where customer records contain several data quality issues, including:

* Duplicate customer records
* Missing email addresses
* Merged name columns
* Non-standardized phone numbers
* Incorrect data types
* Additional calculated fields required for analysis

The objective is to clean and transform the data using Snowflake SQL before identifying inactive customers who haven't made a transaction in the last 90 days. 

---

## 🎯 Project Goal

This project introduces one of the most important responsibilities of a Data Analyst or Data Engineer—**Data Preparation and Data Cleansing**.

Using a realistic business scenario, you'll learn how to identify and fix messy data using Snowflake SQL functions. 

---

## 🛠️ Skills Demonstrated

* Data Cleaning
* Data Preparation
* Data Quality Assessment
* String Manipulation
* Date Transformation
* Duplicate Detection
* Data Standardization
* View Creation
* SQL Query Optimization
* Snowflake SQL

---

## 📂 Project Workflow

### 1. Load Project Data

* Import customer dataset
* Configure Snowflake environment
* Load data using SQL `INSERT` statements

---

### 2. Investigate Data Quality

* Inspect random records
* Analyze data quality
* Use Snowflake contextual statistics
* Identify inconsistencies

**Functions Used**

* `RANDOM()`
* `LIMIT`

---

### 3. Remove Unwanted Characters

Clean inconsistent text values by removing unnecessary spaces and characters.

**Functions Used**

* `TRIM()`
* `LTRIM()`
* `RTRIM()`
* `CONCAT()`

---

### 4. Extract First & Last Names

Split merged customer names into separate columns.

**Functions Used**

* `SPLIT_PART()`

---

### 5. Standardize Phone Numbers

Normalize phone number formatting by removing unwanted prefixes and symbols.

**Functions Used**

* `LTRIM()`

---

### 6. Convert Text to Date

Transform string values into proper SQL date format.

**Functions Used**

* `TO_DATE()`

---

### 7. Create Calculated Columns

Calculate the number of days since each customer's last transaction.

**Functions Used**

* `DATEDIFF()`
* `CURRENT_DATE()`

---

### 8. Handle Missing & Duplicate Data

* Detect duplicate customers
* Correct missing values
* Improve overall data quality

---

### 9. Build a Reusable View

Create a SQL View containing cleaned customer data for future analysis.

---

### 10. Business Analysis

Identify inactive customers who have not made a transaction within the last **90 days**. 

---

## 📚 SQL Functions Covered

| Category         | Functions                                                  |
| ---------------- | ---------------------------------------------------------- |
| String Functions | `TRIM()`, `LTRIM()`, `RTRIM()`, `CONCAT()`, `SPLIT_PART()` |
| Date Functions   | `TO_DATE()`, `DATEDIFF()`, `CURRENT_DATE()`                |
| Query Functions  | `RANDOM()`, `LIMIT`                                        |
| Data Engineering | Views, Data Standardization, Data Cleansing                |

---

## 📁 Repository Structure

```text
.
├── SQL/
│   ├── 01_load_data.sql
│   ├── 02_data_quality_check.sql
│   ├── 03_remove_unwanted_characters.sql
│   ├── 04_extract_names.sql
│   ├── 05_standardize_phone.sql
│   ├── 06_extract_dates.sql
│   ├── 07_calculated_columns.sql
│   ├── 08_remove_duplicates.sql
│   ├── 09_create_view.sql
│   └── 10_inactive_customers.sql
├── datasets/
├── screenshots/
├── README.md
└── LICENSE
```

---

## 🚀 Learning Outcomes

By completing this project, you will be able to:

* Clean messy datasets using Snowflake SQL
* Detect and resolve data quality issues
* Standardize inconsistent values
* Transform string data into structured formats
* Work with SQL date functions
* Create reusable SQL Views
* Prepare datasets for reporting and analytics
* Apply industry-standard data preparation techniques

---

## 🧰 Technologies Used

* Snowflake
* SQL
* Data Cleaning
* Data Transformation
* Data Engineering

---

## 🎓 Course

**Guided Project:** *Data Cleaning in Snowflake: Techniques to Clean Messy Data* (Coursera) 

---

## 👨‍💻 Author

**Saikat Pal**

---

## ⭐ If you found this project helpful...

Give this repository a ⭐ and feel free to fork it to practice more Snowflake SQL data engineering projects.

