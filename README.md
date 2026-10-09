
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
|------------|---------|
| *Filename* | **[employee_attendance_dashboard_cleaned_new9.csv](PASTE_CLEANED_DATASET_LINK_HERE)** |
| *Google Colab Notebook — Data Cleaning* | **[Employee Attendance Data Cleaning](PASTE_DATA_CLEANING_COLAB_LINK_HERE)** |
| *Google Colab Notebook — Data Analysis* | **[Employee_DataAnalysis.ipynb](PASTE_DATA_ANALYSIS_COLAB_LINK_HERE)** |
| *Kaggle Notebook* | **[Employee Attendance — Swastika Ghosal](PASTE_KAGGLE_NOTEBOOK_LINK_HERE)** |
| *Total Records* | **55,374** |
| *Unique Employees* | **980** |
| *Primary Keys / Identifiers* | `attendance_id`, `employee_id` |
| *Source of Data* | **[employee_attendance_bangalore_q1_2026.csv](PASTE_RAW_DATASET_LINK_HERE)** |
| *Analysis Notebook (`.ipynb`)* | **[Employee_DataAnalysis.ipynb](PASTE_GITHUB_ANALYSIS_NOTEBOOK_LINK_HERE)** |
| *Dashboard* | **[Employee Attendance Analytics Dashboard](PASTE_LOOKER_STUDIO_DASHBOARD_LINK_HERE)** |


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
