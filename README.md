# Employee Attendance, Login & Logout Data — Bangalore

Employee attendance and productivity analytics for Bangalore Q1 2026 using Python, Pandas, statistical analysis, data visualization, and Looker Studio dashboards.

---

## Project Overview

This project analyzes employee attendance, working hours, productivity, overtime, work modes, leave patterns, and workforce distribution for employees in Bangalore during Q1 2026.

The project follows a complete data analytics workflow:

- Raw dataset collection
- Data cleaning and preprocessing
- Feature engineering
- Exploratory data analysis
- Statistical analysis
- Data visualization
- Hypothesis testing
- Interactive dashboard development
- Reporting and documentation

---

## Dataset

The project uses an Employee Attendance dataset covering Bangalore for Q1 2026.

### Dataset Details

| Attribute | Details |
|---|---|
| Location | Bangalore |
| Period | Q1 2026 |
| Records | 55,374 |
| Employees | 980 |
| Departments | 10 |
| Raw Columns | 22 |
| Cleaned Columns | 41 |

The dataset contains employee information, attendance records, login and logout timestamps, working hours, break duration, productive hours, late arrival, early exit, overtime, work mode, shift type, and leave information.

---

## Project Structure

```text
Employee-Attendance-Login-Logout-Data-Bangalore/
│
├── 1_Dataset/
│   ├── 1_Raw_Dataset/
│   │   ├── employee_attendance_bangalore_q1_2026.csv
│   │   └── README.md
│   │
│   ├── 2_Data Cleaning/
│   │   ├── Employee_Attendance_Bangalore_q1_2026(DataCleaning).ipynb
│   │   └── README.md
│   │
│   └── 3_Cleaned_Dataset/
│       ├── employee_attendance_dashboard_cleaned_new9.csv
│       └── README.md
│
├── 2_Data_Analysis/
│   ├── Employee_DataAnalysis.ipynb
│   └── README.md
│
├── 3_Dashboards/
│   ├── Employee_Attendance_Dashboard_Page1.png
│   ├── Employee_Attendance_Dashboard_Page2.png
│   ├── Employee_Attendance_Dashboard_Page3.png
│   └── README.md
│
├── 4_Reports/
│   ├── Analysis_Outputs/
│   ├── Dashboard_Images/
│   └── README.md
│
└── README.md
---

## Dashboard Preview

### Page 1 — Dashboard Overview

![Employee Attendance Dashboard — Page 1](3_Dashboards/Employee_Attendance_Dashboard_Page1.png)

### Page 2 — Productivity and Overtime Analysis

![Employee Attendance Dashboard — Page 2](3_Dashboards/Employee_Attendance_Dashboard_Page2.png)

### Page 3 — Attendance and Workforce Analysis

![Employee Attendance Dashboard — Page 3](3_Dashboards/Employee_Attendance_Dashboard_Page3.png)
