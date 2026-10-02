# Employee Attendance — Data Analysis

## Overview

This folder contains the Jupyter Notebook used to perform exploratory data analysis, statistical analysis, and visualization on the cleaned employee attendance dataset.

The analysis focuses on employee attendance patterns, working hours, productivity, work modes, departments, employment types, and other workplace-related variables.

---

## Analysis Notebook

**Notebook:** `Employee_DataAnalysis.ipynb`

The notebook was developed using Python and Google Colab.

The complete analysis workflow, visualizations, statistical tests, and interpretations are documented in the notebook.

### Google Colab

The complete analysis notebook is also available in Google Colab:

[Open Employee Data Analysis Notebook in Google Colab](https://colab.research.google.com/drive/1OausWxHCzMGD6Le33BJ2RbxtAodRh2bI?usp=sharing)

---

## Input Dataset

The analysis is performed using the cleaned employee attendance dataset:

`employee_attendance_dashboard_cleaned_new9.csv`

The cleaned dataset contains:

- **Records:** 55,374
- **Columns:** 41
- **Unique Employees:** 980
- **Departments:** 10
- **Time Period:** Q1 2026
- **Location:** Bangalore
- **Date Range:** 2 January 2026 to 31 March 2026

---

# Analysis Workflow

The notebook follows a structured analysis workflow consisting of eight major steps.

---

## Step 01 — Basic Information About the Dataset

The cleaned employee attendance dataset is loaded and its basic structure is examined.

The following information is checked:

- Number of rows
- Number of columns
- First five records
- Data types of columns
- Basic structure of the dataset

The dataset is loaded into a Pandas DataFrame named `df`.

---

## Step 02 — Identify Column Types

The columns are categorized according to their data types.

The following types of columns are identified:

### Numerical Columns

Numerical columns are identified using their numerical data types.

These columns are used for statistical calculations and numerical analysis.

### Categorical Columns

Categorical columns are identified to analyze employee groups, departments, work modes, attendance status, employment types, and other categorical information.

### Date/Time Columns

Date and time columns are identified for temporal analysis.

These include variables such as:

- `date_of_joining`
- `attendance_date`
- `login_timestamp`
- `logout_timestamp`

### ID Columns

Identifier columns are identified separately, including:

- `attendance_id`
- `employee_id`

ID columns are not treated as analytical numerical variables.

---

## Step 03 — Checking Data Types and Missing Values

The data types and missing values are examined separately for:

- Numerical columns
- Categorical columns
- Date/Time columns
- ID columns

This step helps verify the data structure and identify missing values before performing further analysis.

---

## Step 04 — Numerical Summary Statistics

Descriptive statistics are calculated for the selected numerical variables.

The analysis includes:

- Count
- Mean
- Standard deviation
- Minimum
- 25th percentile
- Median
- 75th percentile
- Maximum
- Mode
- Skewness
- Kurtosis

ID-like numerical columns are excluded from statistical analysis because their numerical values represent identifiers rather than measurable quantities.

---

# Step 05 — Univariate Analysis

Univariate analysis is performed to study individual variables separately.

The following analyses are included:

## 5.1 — Distribution of Numerical Variables

Histograms are used to examine the distributions of important numerical variables such as:

- `total_hours_worked`
- `break_duration_mins`
- `net_productive_hours`
- `late_arrival_mins`
- `early_exit_mins`
- `overtime_hours`
- `productivity_ratio`

## 5.2 — Boxplot Analysis of Numerical Variables

Boxplots are used to examine:

- Distribution
- Median
- Quartiles
- Variability
- Potential outliers

for selected numerical variables.

## 5.3 — Statistical Summary of Numerical Variables

A statistical summary is created containing:

- Mean
- Median
- Standard deviation
- Mode
- Skewness
- Kurtosis

## 5.4 — Categorical Variable Analysis

Categorical variables are analyzed using frequency-based visualizations.

The analysis includes:

- Department distribution
- Work mode distribution
- Attendance status distribution

---

# Step 06 — Bivariate Analysis

Bivariate analysis is used to examine relationships between two variables.

The analysis is divided into three categories.

## 6.1 — Numerical vs Numerical

The following relationships are examined:

### 6.1.1 — Total Hours Worked vs Net Productive Hours

A scatter plot and Pearson correlation are used to examine the relationship between total hours worked and net productive hours.

### 6.1.2 — Overtime Hours vs Net Productive Hours

The relationship between overtime hours and net productive hours is examined.

### 6.1.3 — Break Duration vs Productivity Ratio

The relationship between break duration and productivity ratio is analyzed.

### 6.1.4 — Late Arrival Minutes vs Total Hours Worked

The relationship between late arrival and total hours worked is examined.

### 6.1.5 — Early Exit Minutes vs Net Productive Hours

The relationship between early exit minutes and net productive hours is analyzed.

---

## 6.2 — Numerical vs Categorical

Numerical variables are compared across categorical groups.

The following comparisons are performed:

### 6.2.1 — Late Arrival Minutes vs Department

Late arrival patterns are compared across departments.

### 6.2.2 — Net Productive Hours vs Work Mode

Net productive hours are compared across different work modes.

### 6.2.3 — Net Productive Hours vs Department

Net productive hours are compared across departments.

### 6.2.4 — Overtime Hours vs Department

Overtime hours are compared across departments.

### 6.2.5 — Productivity Ratio vs Employment Type

Productivity ratio is compared across different employment types.

---

## 6.3 — Categorical vs Categorical

Cross-tabulation and 100% stacked bar charts are used to examine relationships between categorical variables.

The following relationships are analyzed:

### 6.3.1 — Department vs Work Mode

The distribution of work modes is compared across departments.

### 6.3.2 — Department vs Attendance Status

Attendance status proportions are compared across departments.

### 6.3.3 — Shift Type vs Attendance Status

Attendance status proportions are compared across different shift types.

### 6.3.4 — Employment Type vs Work Mode

Work mode composition is compared across employment types.

---

# Step 07 — Multivariate Analysis

Multivariate analysis is used to examine relationships among multiple variables simultaneously.

The following techniques are included:

## 7.1 — Pair Plot

A pair plot is created using selected numerical variables:

- `total_hours_worked`
- `break_duration_mins`
- `net_productive_hours`
- `late_arrival_mins`

The pair plot is used to examine relationships, distributions, trends, and potential outliers.

A sample of up to 800 records is used for improved readability.

## 7.2 — Correlation Heatmap

A correlation heatmap is created using:

- `total_hours_worked`
- `break_duration_mins`
- `net_productive_hours`
- `late_arrival_mins`
- `early_exit_mins`
- `overtime_hours`
- `tenure_days`

The heatmap provides an overall view of the strength and direction of linear relationships among the selected numerical variables.

## 7.3 — Grouped Box Plot

A grouped box plot is used to examine late arrival minutes across:

- Department
- Work Mode

The analysis focuses on the top five departments based on the number of records.

## 7.4 — Net Productive Hours Distribution by Department

A faceted histogram is used to compare the distribution of net productive hours across the top five departments.

## 7.5 — Multivariate Analysis Summary

The multivariate analysis combines numerical and categorical variables to provide a broader understanding of employee working patterns and productivity.

---

# Step 08 — Hypothesis Testing

Hypothesis testing is performed to determine whether observed relationships or differences are statistically significant.

The significance level used in the hypothesis tests is:

```text
α = 0.05