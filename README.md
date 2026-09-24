# HR Dashboard

An interactive Power BI dashboard for analyzing HR data, covering salaries, employment status, gender and job-level distribution, and employee engagement scores.

## Overview

This dashboard provides a comprehensive view of employee data through a set of visuals that show:

- Total annual salary
- Total number of employees
- Employment status per employee (Active / Inactive)
- Salary distribution by education level
- Salary distribution by gender and job level
- Top 10 employees by engagement score
- Top 10 managers by total salary under their supervision

## Data Source

The data was prepared and cleaned using **Power Query** before being loaded into Power BI. Cleaning steps included:

- Removing rows and columns with errors (Remove Errors / Removed Columns)
- Replacing incorrect or blank values (Replace Values)
- Text formatting (Capitalize Each Word, Trimmed Text)
- Changing data types (Changed Type) for numeric and date columns
- Extracting additional fields such as hire year (Extracted Year from hire_date)
- Splitting the Gender column into two separate columns (Male / Female) using a Custom Column

## Key Dashboard Components (Visuals)

| Component | Description |
|---|---|
| Sum of Annual Salary | Total annual salary across all employees |
| Total Employees Number | Total count of registered employees |
| Employee Statuses | Detailed table showing each employee's status (Active/Inactive) with their ID |
| Salary Per Education Level | Salary distribution by educational qualification (Bachelor's, Master's, Associate's...) |
| Annual Salary per Gender and Job Level | Salary comparison by gender and job level (Manager, Mid, Senior) |
| Top 10 Engagement Score Employees | Top 10 employees ranked by engagement score |
| Top 10 Salary Managers | Top 10 managers ranked by total salary of their team |

## Tools Used

- **Power Query**: Data cleaning and transformation
- **Power BI Desktop**: Building interactive reports and visuals
- **DAX**: Calculating measures (sums, averages, etc.)

## How to Use

1. Open the Power BI file (`.pbix`)
2. From the **Home > Refresh** tab, refresh the data if the source has changed
3. Use the filters available on each visual (Top N, Filters on this visual) to control what's displayed
4. Click on any part of a chart to apply cross-filtering across the rest of the dashboard

## Notes

- The dashboard can be continuously refreshed as new data is added to the source file
- Some charts (like Top 10) use a **Top N** filter type to display only the highest values instead of the full dataset
