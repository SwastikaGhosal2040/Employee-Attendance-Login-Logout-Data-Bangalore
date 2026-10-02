# Employee Attendance — Data Cleaning

## Overview

This folder contains the Jupyter Notebook used to inspect, clean, preprocess, and transform the raw employee attendance dataset.

The cleaned dataset generated through this notebook is used for further exploratory data analysis, statistical analysis, visualization, and dashboard development.

---

## Data Cleaning Notebook

**Notebook:** `Employee_Attendance_Bangalore_q1_2026(DataCleaning).ipynb`

The notebook was developed using Python and Google Colab.

The complete data cleaning and preprocessing workflow is documented in the notebook.

### Google Colab

The complete notebook is also available in Google Colab:

[Open Data Cleaning Notebook in Google Colab](https://colab.research.google.com/drive/1Mz_JOmS14CceyohfSwh79eqbe_-arH9D?usp=sharing)

---

## Input Dataset

The raw dataset used in this notebook is:

`employee_attendance_bangalore_q1_2026.csv`

The dataset contains employee attendance records for Bangalore for Q1 2026.

### Dataset Information

- **Location:** Bangalore
- **Time Period:** Q1 2026
- **Date Range:** 2 January 2026 to 31 March 2026
- **Records:** 55,374
- **Columns in Raw Dataset:** 22
- **Unique Employees:** 980
- **Departments:** 10

---

# Data Cleaning Workflow

The notebook follows a structured data-cleaning and preprocessing workflow.

## Phase 1 — Inspecting the Raw Dataset

The raw dataset is first loaded and inspected to understand its structure and data quality.

The following checks are performed:

### 1. Importing Required Libraries

The required Python libraries are imported for data manipulation and numerical operations.

- Pandas
- NumPy

### 2. Loading the Dataset

The raw CSV dataset is loaded into a Pandas DataFrame.

### 3. Displaying the First Five Records

The first five rows of the dataset are displayed to understand the initial structure and values.

### 4. Checking Dataset Shape

The number of rows and columns is checked.

### 5. Checking Column Names

The names of all columns are examined.

### 6. Checking Dataset Information

The dataset structure, data types, non-null values, and memory usage are examined.

### 7. Generating Basic Statistics

Descriptive statistics are generated for the numerical variables.

### 8. Checking Missing Values

Missing values are identified for each column.

### 9. Checking Duplicate Records

Completely duplicated rows are checked.

### 10. Checking ID Columns

The uniqueness and structure of `attendance_id` and `employee_id` are examined.

### 11. Checking Data Types

The data types of all columns are examined to identify columns that require conversion or preprocessing.

### 12. Checking Memory Usage

Memory usage of the DataFrame is examined.

### 13. Checking Unique Values

Unique values in the dataset are examined to understand categorical variables and their possible values.

---

# Phase 2a — Data Cleaning and Preparation

After the initial inspection, the dataset is prepared for analysis.

## 1. Cleaning Column Names

Extra spaces from column headers are removed to maintain consistent column names.

## 2. Cleaning Text Columns

Leading and trailing spaces are removed from text-based columns to maintain consistency in categorical values.

## 3. Converting Date and Time Columns

The following columns are converted into the appropriate datetime format:

- `date_of_joining`
- `attendance_date`
- `login_timestamp`
- `logout_timestamp`

Invalid date/time values are handled using appropriate conversion.

## 4. Checking Date/Time Conversion

The data types of the date/time columns are verified after conversion.

Missing values in the converted date/time columns are also checked.

## 5. Verifying ID Columns

The attendance and employee identifier columns are examined to ensure that they can be used appropriately for further analysis.

---

# Phase 2b — Feature Engineering

Additional analytical columns are created from the existing dataset.

These derived features make the dataset more suitable for analysis and dashboard development.

## 1. Joining Year

`Joining_Year` is created by extracting the year from `date_of_joining`.

## 2. Employee Tenure in Years

`Employee_Tenure_Years` is created to represent the employee's tenure in years.

## 3. Attendance Month

`Attendance_Month` is created by extracting the month from `attendance_date`.

## 4. Attendance Weekday

`Attendance_Weekday` is created by extracting the weekday from `attendance_date`.

The resulting values represent:

- Monday
- Tuesday
- Wednesday
- Thursday
- Friday
- Saturday
- Sunday

## 5. Login Hour

`Login_Hour` is created by extracting the hour from `login_timestamp`.

## 6. Logout Hour

`Logout_Hour` is created by extracting the hour from `logout_timestamp`.

## 7. Late Arrival Flag

`Late_Arrival_Flag` is created to identify whether an employee arrived late.

- `Late` → A late arrival was recorded.
- `On Time` → No late arrival was recorded.

## 8. Overtime Flag

`Overtime_Flag` is created to identify whether overtime was recorded.

- `Yes` → Overtime was recorded.
- `No` → No overtime was recorded.

## 9. Productivity Category

`Productivity_Category` is created using `net_productive_hours`.

The following categories are used:

| Net Productive Hours | Productivity Category |
|---|---|
| 8 hours or more | Highly Productive |
| 6 to less than 8 hours | Moderately Productive |
| Less than 6 hours | Low Productive |

## 10. Late Arrival Indicator

`is_late` is created as a numerical indicator.

- `1` → Late
- `0` → On Time

## 11. Early Exit Indicator

`is_early_exit` is created as a numerical indicator.

- `1` → Early exit recorded
- `0` → No early exit

## 12. Overtime Hours Paid

`overtime_hours_paid` is created from the overtime information for further analysis.

## 13. Productivity Ratio

`productivity_ratio` is created using the following formula:

```text
Productivity Ratio = Net Productive Hours / Total Hours Worked