HR Analytics & Attrition Insights Dashboard

Domain: Human Resources | Workforce Analytics
Tool: Power Bi|Excel
Project Overview

This project provides a comprehensive end-to-end data analysis of workforce dynamics, attrition trends, compensation structures, and employee performance across an enterprise organization. Utilizing a multi-table relational schema containing 551 unique employee records, the dataset was cleaned, modeled, and visualized in Power BI to uncover key driver metrics for talent retention and workforce stability.

🎯 Project Objectives

   1. Monitor Attrition & Headcount Dynamics
Track real-time active headcount and identify high-risk departments experiencing elevated turnover rates.

  2. Evaluate Compensation Parity
Analyze salary distributions, adjustments, and merit increases across departments and job roles to ensure competitive pay structures.

  3. Assess Employee Performance
Correlate performance scores and competency metrics (communication, teamwork, problem-solving) with turnover risk.

 4. Analyze Internal Career Mobility
Track job title changes, promotions, and departmental movement over time using historical logs.

Data Sources & Architecture

The analysis is powered by a relational data model with primary and foreign key links across 4 core entities:

    EmployeeMaster(551 records): Core employee profiles, hire/termination dates, status, base salary, and ratings.
    Compensation History : Historical salary change logs, new salary levels, and raise reasons (Merit vs. Promotion).
    Job History : Internal title transitions and department history.  
    Performance Reviews : Multi-dimensional review scores (Overall, Communication, Teamwork, Problem-Solving).
Problem Statement

Identify which departments and job titles exhibit the highest attrition rates.
Evaluate if pay disparities or lack of promotions contribute to employee termination.
3.Measure workforce engagement and performance distributions across various business units.
Enable HR leadership to make data-driven decisions on retention strategies and salary benchmarking.
Attribute Details (EmployeeMaster)

| Attribute Name | Data Type | Description |

| EmployeeID | Text | Unique identifier for each employee |
| FullName | Text | Employee full name |
| Department | Text | Finance,Human Resource,IT |
| JobTitle | Text | Current designation/role |
| Email | Text | Corporate email address |
| Gender | Text | Male / Female / Non-binary |
| HireDate | Text | Date of employment commencement |
| TerminationDate | Text | Date of exit (if applicable) |
| Salary | Currency | Base annual compensation |
| ManagerID | Text | Unique identifier of direct manager |
| PerformanceRating | Integer | Overall rating score (1–5 scale) |
| Status | Text | Active / Terminated |

🧹 Preprocessing & Transformation Steps

Data Cleaning: Imputed missing dates, standardized text formatting, and assigned strict data types in Power Query.
Relational Modeling: Established 1-to-Many ( 1:N ) relationships between Employee Master and history tables.
DAX Measures: Formulated measures for active headcount, turnover rate, average salary, and review score aggregations.
Excel Pivot Validation: Created reference summary pivots and macros for data validation and initial exploratory data analysis.
📈 Performance & Workforce Insights
🏢 Overall Headcount: 551 total employees (484 Active, 67 Terminated), representing an overall attrition rate of 12.16%.

🚨 High-Turnover Departments:

IT Support logged the highest attrition rate at 18.97%.

Sales & Logistics followed closely with 15.87% attrition each.

🛡️ Most Stable Department: Research & Development (R&D) maintained the lowest turnover rate at 5.63%.

💰 Salary Overview: Average base salary across the organization is ₹89,867, with highest average compensation in Sales (₹121,213) and Quality Control (₹110,709).

⭐ Performance Distribution: Average overall performance score across the workforce stands at 3.53 / 5.00.

🧠 Conclusion
The integrated Excel & Power BI HR Analytics Dashboard transforms raw HR logs into actionable workforce strategy insights. Key findings highlight the need for targeted retention strategies in high-attrition units like IT Support and Sales, while aligning compensation structures with performance benchmarks to foster long-term employee engagement.

