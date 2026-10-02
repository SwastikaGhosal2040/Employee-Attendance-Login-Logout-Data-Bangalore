# Employee Attendance Analytics Dashboard

This folder contains the visual dashboard developed in **Looker Studio** for analyzing employee attendance, productivity, working patterns, overtime, leave records, and workforce distribution for **Bangalore, Q1 2026**.

The dashboard is presented across three pages. Each page focuses on a different aspect of employee attendance and workforce analytics.

---

## Live Looker Studio Dashboard

The interactive version of the dashboard can be accessed through the link below:

**[Open Employee Attendance Analytics Dashboard in Looker Studio](https://datastudio.google.com/reporting/ef773827-657e-4f0d-bcf9-c6d3325d0f47)**

> **Note:** The Looker Studio report may require appropriate viewing access. If the report does not open, the report owner should enable the required sharing/viewing permissions.

The screenshots below are included so that the dashboard can also be viewed directly from this GitHub repository.

---

# Dashboard Pages

## Page 1 — Attendance and Productivity Overview

![Employee Attendance Dashboard - Page 1](Employee_Attendance_Dashboard_Page1.png)

### Purpose

Page 1 provides an overall view of employee attendance, working hours, productivity, late arrivals, early exits, overtime, work mode, office location, and employee distribution.

### Filters

The page includes filters for:

- Attendance Month
- Department
- Designation
- Employment Type
- Office Location
- Shift Type
- Work Mode
- Attendance Status
- Gender
- Weekday

These filters allow the dashboard to be viewed for selected employee groups or working conditions.

### Key Performance Indicators

| KPI | Value |
|---|---:|
| Total Employees | 980 |
| Attendance Rate | 95.24% |
| Average Hours Worked | 8.72 |
| Average Net Productive Hours | 7.73 |
| Late Arrival Rate | 49.63% |
| Early Exit Rate | 32.39% |
| Average Overtime Hours | 0.63 |

### Visualizations

**Work Mode Distribution**  
Shows the distribution of attendance records across Work From Office, Work From Home, Not Applicable, and Client Site.

**Overall Productivity Ratio**  
Displays the overall productivity ratio as a gauge, with the dashboard showing approximately **88.3%**.

**Attendance Records by Office Location**  
Compares attendance records across office locations such as Koramangala HQ, Whitefield Tech Park, HSR Layout Hub, Indiranagar Annexe, and Electronic City Campus.

**Employee Distribution by Employment Type & Shift Type**  
Shows the distribution of employees across employment types and different shift types.

---

## Page 2 — Shift, Overtime and Department Analysis

![Employee Attendance Dashboard - Page 2](Employee_Attendance_Dashboard_Page2.png)

### Purpose

Page 2 focuses on shift-wise late arrival, overtime, net productive hours, and workforce distribution across departments.

### Filters

The page includes filters for:

- Attendance Month
- Department
- Designation

### Key Performance Indicators

| KPI | Value |
|---|---:|
| Total Employees | 980 |
| Attendance Rate | 95.24% |
| Average Hours Worked | 8.72 |
| Early Exit Rate | 32.39% |

### Visualizations

**Average Late Arrival by Shift Type**  
Compares average late-arrival minutes across the available shift types:

- Early (08:00–17:00)
- General (09:30–18:30)
- Flexible (10:30–19:30)
- Mid (11:00–20:00)
- Late/US Overlap (14:00–23:00)

**Impact of Overtime on Net Productive Hours**  
A scatter plot is used to examine the relationship between overtime hours and net productive hours. The plotted employee records show how these two numerical variables vary together.

**Average Overtime Hours by Department**  
Compares average overtime hours across departments.

**Workforce Distribution by Department**  
A treemap is used to visualize the relative workforce distribution across departments.

---

## Page 3 — Leave and Department-Level Analysis

![Employee Attendance Dashboard - Page 3](Employee_Attendance_Dashboard_Page3.png)

### Purpose

Page 3 provides a detailed view of leave records, employment type, attendance records by department, and average net productive hours by department.

### Filters

The page includes filters for:

- Employment Type
- Office Location
- Shift Type

### Key Performance Indicators

| KPI | Value |
|---|---:|
| Total Employees | 980 |
| Productivity Ratio | 88.34% |
| Average Net Productive Hours | 7.73 |
| Average Hours Worked | 8.72 |
| Attendance Rate | 95.24% |

### Visualizations

**Leave Type Distribution**  
Shows the number of records for different leave categories, including:

- Casual Leave
- Sick Leave
- Earned Leave
- Loss of Pay
- Work From Home Comp-Off
- Parental Leave
- Bereavement Leave
- Marriage Leave

**Employment Type Distribution**  
A donut chart shows the distribution of employees across Full-Time, Contract, Intern, and Part-Time employment types.

**Attendance Records by Department**  
Compares the number of attendance records across departments.

**Average Net Productive Hours by Department**  
Compares average net productive hours across departments.

---

# Dashboard Design and Functionality

The dashboard was designed to provide interactive exploration of employee attendance data through:

- KPI cards for key performance indicators
- Interactive filters for employee and attendance segments
- Bar charts for department and category comparisons
- Pie and donut charts for distribution analysis
- A gauge chart for overall productivity ratio
- A scatter plot for overtime and productivity analysis
- A treemap for workforce distribution
- A detailed table for employment type and shift distribution

The dashboard supports both high-level monitoring and detailed department, shift, employment, and attendance analysis.

---

# Tools Used

- **Looker Studio** — Dashboard development and visualization
- **Google Sheets / CSV data** — Data source and prepared dataset
- **Python / Pandas** — Data cleaning and preprocessing
- **Statistical analysis** — Used in the analysis stage to examine relationships and differences in the attendance data

---

# Dashboard Screenshots

| Page | Description |
|---|---|
| Page 1 | Attendance and Productivity Overview |
| Page 2 | Shift, Overtime and Department Analysis |
| Page 3 | Leave and Department-Level Analysis |

The image files are stored directly in this folder so they can be viewed from the GitHub repository without opening the external dashboard.

---

# Project Workflow

The dashboard is part of a larger Employee Attendance Analytics workflow:

```text
Raw Dataset
    ↓
Data Cleaning & Preprocessing
    ↓
Feature Engineering
    ↓
Data Analysis & Statistical Testing
    ↓
Looker Studio Dashboard