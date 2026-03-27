
# Global Survey Data Analysis Dashboard (Power BI)

##  Project Overview
In this project, I worked with a global survey dataset containing responses from people across different countries, industries and roles.  

The aim was to take messy, real-world data and transform it into a clean, interactive Power BI dashboard that provides meaningful insights.

---

##  Dataset
The dataset was provided as a raw CSV file and includes:

###  Professional Information
Job Title  
Industry  
Favorite Programming Language  

###  Salary
- Stored as text ranges (e.g., "106k-125k")

###  Workplace Sentiment (0–10 scale)
Salary satisfaction  
Work-life balance  
Management satisfaction  

---

## Data Cleaning (Power Query)

### 1. Standardising Categories
Some responses were inconsistent because users selected "Other" and entered custom text.

**Steps taken:**
Split columns using delimiters like `(` and `:`
Grouped similar responses into main categories:
  Data Analyst  
  Data Scientist  
  Student  

 Result: Cleaner and more consistent data for analysis.

---

### 2. Converting Salary to Numeric Values
Salary data was originally text-based, which made it unusable for calculations.

**Approach:**
 Split salary into minimum and maximum values  
 Calculated the average salary using:
 
Average Salary = (Min Salary + Max Salary) / 2

 Converted the column to a decimal number  

 Result: Salary data could now be used in visuals and comparisons.

---

##  Dashboard Visualisations

###  Key Metrics
**Total Survey Takers:** 630  
 **Average Age:** ~30 years  

---

###  Insights

**Average Salary by Job Title (Bar Chart)**  
  → Data Scientists earn the highest (~$93k)

  **Favourite Programming Language (Column Chart)**  
  → Python is the most popular

  **Country Distribution (Tree Map)**  
  → Acts as a filter for the entire dashboard

  **Happiness Levels (Gauge Charts)**  
  → Shows satisfaction with salary and work-life balance

  **Difficulty Breaking into Data (Donut Chart)**  
  → Red = Difficult, Blue = Easy

---
The dashboard allows users to:
Compare salaries across countries (e.g., US vs UK vs India)  
Identify popular programming languages  
Understand global job satisfaction trends  


