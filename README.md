
# Employee Attendance, Login & Logout Data — Bangalore

Employee attendance and productivity analytics for Bangalore Q1 2026 using Python, Pandas, statistical analysis, data visualization, and Looker Studio dashboards.

---

## Project Overview

The objective of this project is to analyze employee attendance, working hours, productivity, overtime, work modes, leave patterns, and workforce distribution for Bangalore during Q1 2026. The project aims to identify workforce patterns and provide meaningful insights through data cleaning, exploratory data analysis, statistical analysis, and interactive visualization.

The analysis is presented through an interactive **Employee Attendance Analytics Dashboard**, developed using Looker Studio and organized into three pages:

- **Page 1 — Attendance and Productivity Overview:** Summarizes employee attendance, working hours, productivity, work modes, and workforce distribution across office locations and shifts.
- **Page 2 — Shift, Overtime and Department Analysis:** Examines shift-wise late arrivals, overtime patterns, the relationship between overtime and net productive hours, and department-wise workforce distribution.
- **Page 3 — Leave and Department-Level Analysis:** Highlights leave patterns, employment type distribution, department-wise attendance records, and average net productive hours across departments.

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

![Employee Attendance Analytics Cover Photo](CoverPhoto_Employee.png)

---

## Dataset

The project uses an Employee Attendance dataset covering Bangalore for Q1 2026.

### Dataset Details

| Attribute | Details |
|---|---|
| Location | Bangalore |
| Period | Q1 2026 (January–March 2026) |
| Records | 55,374 |
| Unique Employees | 980 |
| Departments | 10 |
| Raw Columns | 22 |
| Cleaned Columns | 41 |

The dataset contains employee information, attendance records, login and logout timestamps, working hours, break duration, productive hours, late arrivals, early exits, overtime, work modes, shift types, and leave information.

---

## File Details

| Attribute | Details |
|---|---|
| **Raw Dataset** | [employee_attendance_bangalore_q1_2026.csv](https://docs.google.com/spreadsheets/d/1jT9biitZJI6d6yCA7TTaTouqdqY65MFXj076heiqV5U/edit?usp=sharing) |
| **Cleaned Dataset** | [employee_attendance_dashboard_cleaned_new9.csv](https://docs.google.com/spreadsheets/d/1OeTd_wJds3kVfQUhpa9hTu1P_v3u-3dOFZSQnqTcY3A/edit?usp=sharing) |
| **Google Colab — Data Cleaning** | [Employee Attendance Data Cleaning Notebook](https://colab.research.google.com/drive/1Mz_JOmS14CceyohfSwh79eqbe_-arH9D?usp=sharing) |
| **Google Colab — Data Analysis** | [Employee Attendance Data Analysis Notebook](https://colab.research.google.com/drive/1OausWxHCzMGD6Le33BJ2RbxtAodRh2bI?usp=sharing) |
| **Kaggle Notebook** | [Employee Attendance — Swastika Ghosal](https://www.kaggle.com/code/swastikaghosal/employee-attendance-swastika-ghosal) |
| **GitHub Analysis Notebook** | [Employee_DataAnalysis.ipynb](https://github.com/SwastikaGhosal2040/Employee-Attendance-Login-Logout-Data-Bangalore/blob/main/2_Data_Analysis/Employee_DataAnalysis.ipynb) |
| **Interactive Dashboard** | [Employee Attendance Analytics Dashboard](https://datastudio.google.com/reporting/ef773827-657e-4f0d-bcf9-c6d3325d0f47) |

---

## Repository Structure

```text
Employee-Attendance-Login-Logout-Data-Bangalore/
│
├── CoverPhoto_Employee.png
├── README.md
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
└── 4_Reports/
    ├── Analysis_Outputs/
    ├── Dashboard_Images/
    └── README.md
```

---

# Dashboard Pages

## Page 1 — Attendance and Productivity Overview

![Employee Attendance Dashboard - Page 1](3_Dashboards/Employee_Attendance_Dashboard_Page1.png)

### Purpose

Page 1 provides an overall summary of employee attendance, working hours, productivity, work modes, office locations, late arrivals, early exits, overtime, and employee distribution.

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
| Productivity Ratio | 88.34% |

### Visualizations

- **Work Mode Distribution:** Shows the distribution of attendance records across Work From Office, Work From Home, Not Applicable, and Client Site.
- **Overall Productivity Ratio:** Displays the overall productivity ratio using a gauge chart.
- **Attendance Records by Office Location:** Compares attendance records across Koramangala HQ, Whitefield Tech Park, HSR Layout Hub, Indiranagar Annexe, and Electronic City Campus.
- **Employee Distribution by Employment Type & Shift Type:** Presents employee counts across employment types and different shift types.

---

## Page 2 — Shift, Overtime and Department Analysis

![Employee Attendance Dashboard - Page 2](3_Dashboards/Employee_Attendance_Dashboard_Page2.png)

### Purpose

Page 2 focuses on shift-wise late arrivals, overtime hours, the relationship between overtime and net productive hours, and workforce distribution across departments.

### Filters

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

- **Average Late Arrival by Shift Type:** Compares average late-arrival minutes across Early, General, Flexible, Mid, and Late/US Overlap shifts.
- **Impact of Overtime on Net Productive Hours:** Uses a scatter plot to visualize the relationship between overtime hours and net productive hours. The observed relationship does not by itself establish causation.
- **Average Overtime Hours by Department:** Compares average overtime hours recorded across departments.
- **Workforce Distribution by Department:** Uses a treemap to compare the relative workforce distribution across departments.

---

## Page 3 — Leave and Department-Level Analysis

![Employee Attendance Dashboard - Page 3](3_Dashboards/Employee_Attendance_Dashboard_Page3.png)

### Purpose

Page 3 provides a detailed view of leave records, employment type distribution, department-level attendance records, and average net productive hours by department.

### Filters

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

- **Leave Type Distribution:** Shows the distribution across Casual Leave, Sick Leave, Earned Leave, Loss of Pay, Work From Home Comp-Off, Parental Leave, Bereavement Leave, and Marriage Leave.
- **Employment Type Distribution:** Uses a donut chart to show the distribution of Full-Time, Contract, Intern, and Part-Time employees.
- **Attendance Records by Department:** Compares attendance record counts across departments.
- **Average Net Productive Hours by Department:** Compares average net productive hours across departments.

---

# Dashboard Design and Functionality

The dashboard supports interactive exploration of employee attendance and productivity data through:

- KPI cards for key performance indicators
- Interactive filters for employee and attendance segments
- Bar charts for category and department comparisons
- Pie and donut charts for distribution analysis
- Gauge chart for overall productivity ratio
- Scatter plot for overtime and productivity analysis
- Treemap for workforce distribution
- Tables for employment type and shift distributions

Together, the three pages provide an overview of attendance, productivity, overtime, leave, shifts, work modes, employment types, and departments.

---

# Tools Used

- **Looker Studio** — Dashboard development and visualization
- **Google Sheets / CSV** — Dataset storage and prepared data
- **Python** — Data processing and analysis
- **Pandas and NumPy** — Data manipulation and numerical analysis
- **Matplotlib and Seaborn** — Data visualization
- **Statistical Analysis** — Analysis of relationships and differences within attendance data
- **Google Colab and Kaggle** — Notebook execution environments
- **GitHub** — Version control and project documentation

---

# Dashboard Files

| File | Description |
|---|---|
| `Employee_Attendance_Dashboard_Page1.png` | Attendance and productivity overview |
| `Employee_Attendance_Dashboard_Page2.png` | Shift, overtime, and department analysis |
| `Employee_Attendance_Dashboard_Page3.png` | Leave and department-level analysis |

---

# Dashboard Preview

The following images provide a visual preview of all three dashboard pages.

### Page 1 — Attendance and Productivity Overview

![Dashboard Preview - Page 1](3_Dashboards/Employee_Attendance_Dashboard_Page1.png)

### Page 2 — Shift, Overtime and Department Analysis

![Dashboard Preview - Page 2](3_Dashboards/Employee_Attendance_Dashboard_Page2.png)

### Page 3 — Leave and Department-Level Analysis

![Dashboard Preview - Page 3](3_Dashboards/Employee_Attendance_Dashboard_Page3.png)

---

**Explore the interactive dashboard:** [Open Employee Attendance Analytics Dashboard](https://datastudio.google.com/reporting/ef773827-657e-4f0d-bcf9-c6d3325d0f47)
