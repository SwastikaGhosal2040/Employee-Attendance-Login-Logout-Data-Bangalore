# Cleaned Dataset — Employee Attendance

## Dataset Overview

This folder contains the cleaned and processed version of the raw employee attendance dataset used for the Employee Attendance Analysis project.

The dataset was prepared through data cleaning, data type conversion, validation, and feature engineering. The cleaned dataset is used for exploratory data analysis, statistical analysis, visualization, and dashboard development.

---

## Dataset File

**File Name:** `employee_attendance_dashboard_cleaned_new9.csv`

**File Format:** CSV

**Location:** Bangalore

**Time Period:** Q1 2026

**Date Range:** 2 January 2026 to 31 March 2026

---

## Dataset Size

- **Total Records:** 55,374
- **Total Columns:** 41
- **Unique Employees:** 980
- **Number of Departments:** 10

---

## Data Cleaning and Preprocessing

The following data-cleaning and preprocessing steps were performed:

- The raw dataset was loaded and inspected.
- Duplicate records were checked.
- Missing values were identified.
- Column data types were examined.
- Date and time columns were converted into appropriate datetime format.
- Numerical and categorical columns were identified.
- ID columns were identified separately.
- Numerical variables were analyzed using descriptive statistics.
- Important numerical variables were examined using distribution plots and boxplots.
- Categorical variables were analyzed using frequency distributions.
- Additional analytical features were created.
- The final cleaned dataset was prepared for further analysis.

---

## Feature Engineering

Additional columns were created from the existing dataset to support analysis.

| Column | Description |
|---|---|
| `Joining_Year` | Year extracted from the employee joining date |
| `Employee_Tenure_Years` | Employee tenure expressed in years |
| `Attendance_Month` | Month extracted from the attendance date |
| `Attendance_Weekday` | Weekday extracted from the attendance date |
| `Login_Hour` | Hour extracted from the login timestamp |
| `Logout_Hour` | Hour extracted from the logout timestamp |
| `Late_Arrival_Flag` | Indicates whether the employee arrived late |
| `Overtime_Flag` | Indicates whether overtime was recorded |
| `Productivity_Category` | Category assigned based on productivity |
| `is_late` | Numeric indicator for late arrival |
| `is_early_exit` | Numeric indicator for early exit |
| `overtime_hours_paid` | Overtime hours considered for payment |
| `productivity_ratio` | Ratio used to represent employee productivity |
| `is_on_leave` | Numeric indicator for leave status |
| `Attendance_Flag` | Numeric indicator related to attendance |
| `tenure_days` | Employee tenure represented in days |
| `attendance_month_num` | Numeric representation of the attendance month |
| `Quarter` | Quarter associated with the attendance record |
| `Attendance_Year` | Year associated with the attendance record |

---

## Main Categories of Information

The cleaned dataset contains information related to:

### Employee Information

- Employee ID
- Employee Name
- Gender
- Department
- Designation
- Employment Type
- Office Location
- Date of Joining

### Attendance Information

- Attendance ID
- Attendance Date
- Attendance Status
- Shift Type
- Work Mode
- Leave Type

### Working Hours

- Login Timestamp
- Logout Timestamp
- Total Hours Worked
- Break Duration
- Net Productive Hours
- Overtime Hours

### Attendance Behaviour

- Late Arrival Minutes
- Early Exit Minutes
- Late Arrival Flag
- Overtime Flag
- Early Exit Indicator

### Productivity

- Productivity Ratio
- Productivity Category
- Net Productive Hours

### Derived Features

- Joining Year
- Employee Tenure
- Tenure Days
- Attendance Month
- Attendance Month Number
- Attendance Weekday
- Attendance Year
- Quarter
- Login Hour
- Logout Hour

---

## Statistical Analysis

The cleaned dataset is used for statistical analysis, including:

- Pearson Correlation
- Independent Samples t-Test
- One-Way ANOVA
- Chi-Square Test

These statistical methods are used to examine relationships, differences, and associations among relevant attendance and productivity variables.

---

## Exploratory Data Analysis

The cleaned dataset is used to create:

- Histograms
- Boxplots
- Countplots
- Pie charts
- Scatter plots
- Pair plots
- Correlation heatmaps
- Grouped boxplots
- Department-wise analysis
- Cross-tabulations
- Distribution analysis

---

## Dashboard

The cleaned dataset is used as a data source for the Employee Attendance Dashboard.

The dashboard analyzes areas such as:

- Employee attendance
- Department-wise information
- Work modes
- Working hours
- Net productive hours
- Overtime
- Late arrivals
- Early exits
- Productivity
- Employee tenure

---

## Data Quality

The cleaned dataset contains:

- **55,374 records**
- **41 columns**
- **980 unique employees**
- **10 departments**

The dataset was validated after data cleaning and feature engineering before being used for further analysis.

---

## Google Sheets

A Google Sheets version of the cleaned dataset is available here:

**[View Cleaned Dataset in Google Sheets](https://docs.google.com/spreadsheets/d/1OeTd_wJds3kVfQUhpa9hTu1P_v3u-3dOFZSQnqTcY3A/edit?usp=sharing)**

The Google Sheet is provided for convenient viewing of the cleaned dataset.

---

## Tools Used

The data cleaning and preprocessing were performed using:

- Python
- Pandas
- NumPy
- Google Colab
- Jupyter Notebook

---

## Relationship with the Raw Dataset

This cleaned dataset was prepared from the original raw employee attendance dataset.

The raw dataset is maintained separately in the `1_Raw_Dataset` folder.

[View Raw Dataset](../1_Raw_Dataset/)

The cleaned dataset is used as the basis for subsequent exploratory data analysis, statistical analysis, visualization, and dashboard development.

---

## Important Note

This file represents the processed and analysis-ready version of the employee attendance dataset.

The original raw dataset is maintained separately and should not be modified.

Further analysis and visualization are performed using this cleaned dataset.