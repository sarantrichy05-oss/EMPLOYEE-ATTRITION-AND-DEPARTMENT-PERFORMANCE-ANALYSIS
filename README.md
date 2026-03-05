# Employee Attrition and Department Performance Analysis

---

## Table of Contents

- Project Overview
- Data Source
- Tools & Technologies
- Data Cleaning & Preparation
- Exploratory Data Analysis (EDA)
- Key Insights
- Recommendations
- How to Use

---

## Project Overview

This project focuses on analyzing Human Resources data related to employee diversity, performance, salary, and attrition to understand employee retention patterns and evaluate department-wise performance.

### Objectives

- Analyze employee attrition and retention trends  
- Compare department-wise salary and performance  
- Evaluate workforce diversity across gender and job levels  
- Support HR decision-making using data-driven insights  

The project demonstrates how structured HR analytics can help organizations identify workforce risks and improve long-term employee stability.

---

## Data Source

- **Source:** Google Dataset Search – HR Analytics / Diversity Dataset  
- **Domain:** Human Resources  
- **Dataset Link:**  
  https://figshare.com/articles/dataset/Human_Resources_csv/28780886?file=53616341  
- **Date Accessed:** 11-04-2025  

### Key Attributes

- Employee_ID  
- Gender  
- Age  
- Department  
- Birth_Date  
- Hire_Date  
- Race  
- Age_Group (Created)  
- Experience_Years  
- Experience_Group (Created)  
- Attrition (Created: 1 = Left, 0 = Active)  

---

## Tools & Technologies

### Microsoft Excel
- Data Cleaning & Transformation  
- Pivot Tables  
- XLOOKUP  
- Feature Engineering  
- Fact & Dimension Table Creation  

### Power BI
- Star Schema Data Modeling  
- DAX Measures  
- Interactive Dashboard Creation  
- Data Visualization  

---

## Data Cleaning & Preparation

The dataset was prepared using the following steps:

### Data Cleaning

- Removed duplicate records  
- Checked and handled blank/missing values  
- Standardized date formats (Birth_Date, Hire_Date)  
- Converted dataset into structured Excel Table  
- Ensured consistency in categorical fields (Department, Gender, Race)  

### Transformation & Feature Engineering

Treated blank Termination_Date as Active employees:

Created Attrition Column:

Created Age Group:

Created Experience Group:

### Pivot Tables Created

- Total Employees by Department  
- Attrition Count by Department  
- Attrition by Age Group  
- Attrition by Experience Group  
- Gender-wise Attrition  

These helped in performing descriptive analysis and identifying patterns.

---

## Data Modeling (Excel → Power BI)

A **Star Schema model** was implemented.

### Fact Table

- Fact_employee_attrition  
  - Employee_ID  
  - Department_ID  
  - Gender_ID  
  - Age_group_ID  
  - Experience_group_ID  
  - Age  
  - Experience  
  - Attrition  

### Dimension Tables

- Dim_Department  
- Dim_Gender  
- Dim_Age_Group  
- Dim_Experience_Group  
- Dim_Employee  

✔ One-to-Many relationships  
✔ Single direction filtering (Dimension → Fact)  
✔ Active relationships  
✔ Surrogate keys fetched using XLOOKUP  

Example:

---

## Exploratory Data Analysis (EDA)

### Business Questions Explored

- Which department has the highest attrition?  
- Do remote employees leave more than headquarters employees?  
- Is attrition higher among specific age groups?  
- How does experience level impact attrition?  
- Is attrition distributed equally across gender?  
- Which hiring periods show higher exits?  

### Major Visualizations Created in Power BI

- Attrition by Department  
- Attrition by Work Location  
- Attrition by Gender  
- Attrition by Age Group  
- Total Employees by Department  
- Total Employees by Work Location  
- Total Employees by Status  
- Attrition Trend by Hire Date  
- Experience Group vs Attrition  

*(Insert dashboard screenshot here in your GitHub repository for better presentation.)*

---

## Key Insights

- Overall attrition rate indicates a noticeable portion of workforce exits.  
- Certain departments show significantly higher attrition levels.  
- Senior age group (46+) shows the highest attrition.  
- Employees with lower experience levels contribute more to exits.  
- Remote and Headquarters employees show variation in attrition patterns.  
- Workforce distribution across departments is uneven.  
- Majority of employees remain active, indicating overall organizational stability.  

---

## Recommendations

- Develop retention strategies for high-risk departments.  
- Improve engagement programs for early-stage employees.  
- Create retention plans for senior employees.  
- Review workload balance in departments with high turnover.  
- Monitor remote vs headquarters retention trends for policy adjustments.  
- Implement workforce planning strategies to address department imbalance.  

---

## How to Use

### Excel File
Open the Excel file to review:
- Cleaned dataset  
- Pivot tables  
- Feature engineering  

### Power BI File
Open the Power BI (.pbix) file to:
- Explore interactive dashboard  
- Use slicers to filter by Department, Gender, Age Group, Experience Group  
- Analyze attrition patterns dynamically  

### Requirements

- Microsoft Excel  
- Power BI Desktop  


