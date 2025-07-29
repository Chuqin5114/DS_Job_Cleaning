# Data Science Job Posting Analysis

### Tool Used
![Python](https://img.shields.io/badge/Python-blue)

### Project Type
![Data Cleaning](https://img.shields.io/badge/Data%20Cleaning-purple)
![Data Transformation](https://img.shields.io/badge/Data%20Transformation-purple)
![Exploratory Data Analysis](https://img.shields.io/badge/Exploratory%20Data%20Analysis-purple)

## Table of Contents
- [Project Overview](#project-overview)  
- [Dataset](#dataset)  
- [Key Steps Performed](#key-steps-performed)  
    - [Data Cleaning](#data-cleaning)  
    - [Data Transformation](#data-transformation)  
    - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)  
- [How to Use](#how-to-use)  
- [Future Work](#future-work)

## Project Overview
This project focuses on cleaning, transforming, and exploring the **"Data Science Job Posting on Glassdoor"** dataset to prepare it for deeper analysis and insights.  
The dataset includes information about various data science job postings such as job titles, salary estimates, company details, job descriptions, and required skills.

---

## Dataset
- **Source:** [Kaggle – Data Science Job Posting on Glassdoor](https://www.kaggle.com/datasets/rashikrahmanpritom/data-science-job-posting-on-glassdoor)  
- **Entries:** 672 rows  
- **Original Columns:** 15  
- **Post-Cleaning:** Dataset expanded with additional **derived features** and **binary skill indicators** (Python, Excel, Tableau, Big Data, Hadoop, Spark, AWS).

---

## Key Steps Performed

### Data Cleaning
- Checked for missing values (**none found**).
- Verified duplicate rows (**none found**).
- Cleaned whitespace in string columns.
- Removed unnecessary columns (`Competitors`).

### Data Transformation
- **Salary Processing:**
  - Cleaned salary strings (removed `$`, `K`, and text).
  - Extracted `min_salary` and `max_salary`.
  - Calculated `avg_salary`.
- **Location Parsing:**
  - Extracted U.S. state from `Location`.
- **Job Title Simplification:**
  - Categorized titles into: **Data Scientist**, **Analyst**, **Engineer**, **Other**.
- **Company Age:**
  - Derived as `2025 - Founded year`.
- **Skill Extraction:**
  - Created binary columns for skills:
    - Python, Excel, Tableau, Big Data, Hadoop, Spark, AWS.

### Exploratory Data Analysis (EDA)
- Visualized company rating distributions.
- Analyzed company age distribution.
- Performed initial skill frequency and salary insights.

---

## How to Use
- Clone the repository
- Install required packages (pandas, numpy, seaborn, matplotlib)
- Run the Jupyter notebook DataScience_Job_Cleaning.ipynb

## Future Work
- Further analysis of salary distributions by state and job category
- More detailed skill requirement analysis
- Company size and revenue impact on salaries
- Natural Language Processing of job descriptions
