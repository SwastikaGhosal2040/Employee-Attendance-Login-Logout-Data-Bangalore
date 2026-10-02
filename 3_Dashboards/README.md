# Employee Attendance Analytics Dashboard

This folder contains the interactive **Employee Attendance Analytics Dashboard** developed using **Looker Studio** for analyzing employee attendance, working hours, productivity, overtime, leave records, work modes, shifts, and department-level workforce patterns for **Bangalore, Q1 2026**.

The dashboard consists of three pages, with each page focusing on a different aspect of employee attendance and workforce analytics.

---

## Live Looker Studio Dashboard

The interactive dashboard can be accessed using the link below:

[Open Employee Attendance Analytics Dashboard in Looker Studio](https://datastudio.google.com/reporting/ef773827-657e-4f0d-bcf9-c6d3325d0f47)

> **Note:** The Looker Studio report may require appropriate viewing permissions. If the dashboard does not open, the report owner should enable the required sharing/viewing access.

The screenshots below provide a static view of the dashboard directly within this GitHub repository.

---

# Dashboard Pages

## Page 1 — Attendance and Productivity Overview

![Employee Attendance Dashboard - Page 1](Employee_Attendance_Dashboard_Page1.png)

### Purpose

Page 1 provides an overall summary of employee attendance, working hours, productivity, work mode, office location, late arrivals, early exits, overtime, and employee distribution.

### Filters

The page provides interactive filters for:

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
Displays the overall productivity ratio using a gauge chart. The dashboard shows an overall productivity ratio of approximately **88.3%**.

**Attendance Records by Office Location**  
Shows the distribution of attendance records across different office locations, including Koramangala HQ, Whitefield Tech Park, HSR Layout Hub, Indiranagar Annexe, and Electronic City Campus.

**Employee Distribution by Employment Type & Shift Type**  
Provides a detailed table showing employee counts across employment types and different shift types.

---

## Page 2 — Shift, Overtime and Department Analysis

![Employee Attendance Dashboard - Page 2](Employee_Attendance_Dashboard_Page2.png)

### Purpose

Page 2 focuses on shift-wise late arrivals, overtime hours, the relationship between overtime and net productive hours, and workforce distribution across departments.

### Filters

The page provides filters for:

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
Compares average late-arrival minutes across different shift types, including Early, General, Flexible, Mid, and Late/US Overlap shifts.

**Impact of Overtime on Net Productive Hours**  
A scatter plot is used to visualize the relationship between overtime hours and net productive hours across employee attendance records.

**Average Overtime Hours by Department**  
Compares the average overtime hours recorded across different departments.

**Workforce Distribution by Department**  
A treemap is used to represent the relative workforce distribution across departments, allowing department sizes to be compared visually.

---

## Page 3 — Leave and Department-Level Analysis

![Employee Attendance Dashboard - Page 3](Employee_Attendance_Dashboard_Page3.png)

### Purpose

Page 3 provides a detailed view of leave records, employment type distribution, department-level attendance records, and average net productive hours by department.

### Filters

The page provides filters for:

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
Shows the number of leave records across different leave categories, including Casual Leave, Sick Leave, Earned Leave, Loss of Pay, Work From Home Comp-Off, Parental Leave, Bereavement Leave, and Marriage Leave.

**Employment Type Distribution**  
A donut chart presents the distribution of employees across Full-Time, Contract, Intern, and Part-Time employment types.

**Attendance Records by Department**  
Compares the number of attendance records across different departments.

**Average Net Productive Hours by Department**  
Compares average net productive hours across departments to provide a department-level view of productivity.

---

# Dashboard Design and Functionality

The dashboard was designed to provide interactive exploration of employee attendance and productivity data through:

- KPI cards for key performance indicators
- Interactive filters for employee and attendance segments
- Bar charts for category and department comparisons
- Pie and donut charts for distribution analysis
- Gauge chart for overall productivity ratio
- Scatter plot for overtime and productivity analysis
- Treemap for workforce distribution
- Detailed tables for employee and shift distributions

The three dashboard pages together provide both an overall summary and detailed views of attendance, productivity, overtime, leave, shifts, work modes, employment types, and departments.

---

# Tools Used

- **Looker Studio** — Dashboard development and visualization
- **Google Sheets / CSV** — Data source and prepared dataset
- **Python / Pandas** — Data cleaning and preprocessing
- **Statistical Analysis** — Analysis of relationships and differences within the attendance data

---

# Dashboard Files

| File | Description |
|---|---|
| `Employee_Attendance_Dashboard_Page1.png` | Attendance and productivity overview |
| `Employee_Attendance_Dashboard_Page2.png` | Shift, overtime, and department analysis |
| `Employee_Attendance_Dashboard_Page3.png` | Leave and department-level analysis |

---

# Project Workflow

The dashboard is part of the following Employee Attendance Analytics workflow:

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
    ↓
Final Reports and Visualizations
