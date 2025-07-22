# Data Science Job Posting Analysis

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

### 1. Data Cleaning
- Checked for missing values (**none found**).
- Verified duplicate rows (**none found**).
- Cleaned whitespace in string columns.
- Removed unnecessary columns (`Competitors`).

### 2. Data Transformation
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

### 3. Exploratory Data Analysis (EDA)
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
