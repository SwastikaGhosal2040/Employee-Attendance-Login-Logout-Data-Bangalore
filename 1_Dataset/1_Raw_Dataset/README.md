# Raw Dataset — Employee Attendance

## Dataset Overview

This folder contains the original raw employee attendance dataset used for the Employee Attendance Analysis project.

The dataset contains employee information, attendance records, department details, employment type, work mode, working hours, break duration, productivity, late arrivals, early exits, overtime, and leave information.

---

## Dataset File

**File Name:** `employee_attendance_bangalore_q1_2026.csv`

**File Format:** CSV

**Location:** Bangalore

**Time Period:** Q1 2026

**Date Range:** 2 January 2026 to 31 March 2026

---

## Dataset Size

- **Total Records:** 55,374
- **Total Columns:** 22
- **Unique Employees:** 980
- **Number of Departments:** 10

---

## Columns in the Dataset

| Column | Description |
|---|---|
| `attendance_id` | Unique identifier for each attendance record |
| `employee_id` | Unique identifier of the employee |
| `employee_name` | Name of the employee |
| `gender` | Gender of the employee |
| `department` | Department of the employee |
| `designation` | Job designation of the employee |
| `employment_type` | Type of employment |
| `office_location` | Office location of the employee |
| `date_of_joining` | Date on which the employee joined |
| `attendance_date` | Date of the attendance record |
| `shift_type` | Shift assigned to the employee |
| `attendance_status` | Attendance status of the employee |
| `work_mode` | Mode in which the employee worked |
| `login_timestamp` | Employee login date and time |
| `logout_timestamp` | Employee logout date and time |
| `total_hours_worked` | Total hours worked by the employee |
| `break_duration_mins` | Break duration in minutes |
| `net_productive_hours` | Net productive working hours |
| `late_arrival_mins` | Number of minutes the employee arrived late |
| `early_exit_mins` | Number of minutes associated with early exit |
| `overtime_hours` | Number of overtime hours |
| `leave_type` | Type of leave associated with the attendance record |

---

## Attendance Status

The raw dataset contains the following attendance records:

| Attendance Status | Records |
|---|---:|
| Present | 51,553 |
| On Leave | 2,635 |
| Half Day | 1,186 |

---

## Work Mode

The dataset contains the following work modes:

| Work Mode | Records |
|---|---:|
| Work From Office | 40,283 |
| Work From Home | 10,906 |
| Client Site | 1,550 |
| Not Applicable | 2,635 |

The `Not Applicable` work mode is associated with the records where the attendance status is `On Leave`.

---

## Employment Type

| Employment Type | Records |
|---|---:|
| Full-Time | 46,113 |
| Contract | 4,543 |
| Intern | 2,837 |
| Part-Time | 1,881 |

---

## Departments

The dataset contains records from the following departments:

- Engineering
- Sales
- Customer Success
- Operations
- Data Science
- Marketing
- Human Resources
- Product Management
- Finance
- Design

---

## Data Quality Check

The raw dataset was inspected before the data-cleaning and analysis stages.

- **No completely duplicated rows were found.**
- All 22 columns are populated except for two timestamp columns.
- `login_timestamp` contains **2,635 missing values**.
- `logout_timestamp` contains **2,635 missing values**.
- The missing login and logout timestamps correspond to the **On Leave** attendance records.
- The remaining columns contain no missing values.

Further data validation, preprocessing, and cleaning were performed separately as part of the project.

---

## Google Sheets

A Google Sheets version of the raw dataset is available here:

**[View Raw Dataset in Google Sheets](https://docs.google.com/spreadsheets/d/1jT9biitZJI6d6yCA7TTaTouqdqY65MFXj076heiqV5U/edit?usp=sharing)**

The Google Sheet is provided for convenient viewing of the raw dataset.

---

## Important Note

This file represents the **raw/unprocessed dataset** used as the starting point for the project.

Data cleaning, preprocessing, exploratory data analysis, statistical analysis, and visualization were performed separately.

The cleaned dataset and analysis files are maintained in their respective project folders.

