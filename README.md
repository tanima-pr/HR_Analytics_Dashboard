# HR Analytics Dashboard

A comprehensive Tableau dashboard that delivers interactive visualizations and insights into workforce trends, employee performance, and HR metrics. This project showcases data modeling, calculated fields, and dashboard design best practices to support evidence-based decision making in human resources.

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Key Features](#key-features)  
3. [Data Sources & Model](#data-sources--model)  
4. [File Structure](#file-structure)  
5. [Prerequisites](#prerequisites)  
6. [Installation & Setup](#installation--setup)  
7. [Usage](#usage)  
8. [Contributing](#contributing)  
9. [License](#license)

---

## Project Overview

This repository contains the packaged Tableau workbook (`HR_Analytics_Dashboard_Tableau.twbx`) which delivers:

- **Workforce Demographics:** Headcount by department, location, and tenure cohort.  
- **Performance & Engagement:** KPI scorecards, performance rating distributions, and engagement survey results.  
- **Turnover & Retention:** Attrition rates over time, voluntary vs. involuntary separations, and predictive risk indicators.  
- **Compensation Analysis:** Salary bands, pay equity comparisons, and benefits utilization trends.  

The dashboard enables HR teams and executives to slice and dice metrics by time period, department, job level, and other key dimensions.

---

## Key Features

- **Executive Summary Dashboard:** High-level KPI tiles (headcount, turnover rate, average tenure) with sparkline trend charts.  
- **Departmental Insights:** Drill-down worksheets showing hiring velocity, attrition drivers, and performance distributions per business unit.  
- **Calculated Fields & Parameters:**  
  - Attrition Rate = (Number of Separations / Average Headcount)  
  - Engagement Score Trends with dynamic sizing parameter  
  - Custom cohorts based on hire date and tenure  
- **Interactive Filters & Actions:** Date sliders, multi-select filters, and dashboard actions for cross-sheet highlighting.  
- **Story Points:** A guided narrative explaining key findings and recommended actions for leadership review.  

---

## Data Sources & Model

| Table / Sheet        | Description                                  |
| -------------------- | -------------------------------------------- |
| `Employees`          | Demographic and job data (hire date, dept, level) |
| `Performance`        | Annual review scores and bonus eligibility     |
| `Engagement`         | Survey responses and engagement indices        |
| `Turnover`           | Separation records with reason codes           |
| `Compensation`       | Salary, bonus, and benefits cost data          |

Joins are configured using common keys (`EmployeeID`, `DepartmentID`), and relationships leverage Tableau’s data model to optimize performance.

---
