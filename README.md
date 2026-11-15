# Telecom Customer Churn Analysis

## Project Overview

Telecom Customer Churn Analysis is a data analytics project focused on cleaning, preprocessing, and transforming telecom customer data using Python. The project aims to prepare a reliable dataset for further exploratory data analysis and customer churn analysis.

## Project Objectives

- Understand and inspect the telecom customer dataset.
- Identify and handle missing values and duplicate records.
- Standardize inconsistent data.
- Detect and inspect potential outliers.
- Convert columns into appropriate data types.
- Create new features for further analysis.
- Prepare cleaned data for future analysis.

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- CSV and Excel

## Dataset Information

The dataset contains telecom customer information, including customer details, service-related information, contract details, charges, tenure, signup dates, and churn status.

## Project Structure

```text
Telecom-Customer-Churn-Analysis/
│
├── data/
│   ├── Telecom Churn raw csv.csv
│   └── Telecom Churn raw excel.xlsx
│
├── cleaned_data/
│   ├── telecom_churn_cleaned_csv.csv
│   └── telecom_churn_cleaned_excel.xlsx
│
├── Telecom Churn Analysis.ipynb
│
└── README.md
```

## Project Workflow

### 1. Data Loading and Inspection
- Loaded the dataset using Pandas.
- Checked the first few records, dataset shape, column information, and descriptive statistics.
- Reviewed column names and data types.

### 2. Data Cleaning and Preprocessing
- Identified missing values and handled selected numerical missing values using median imputation.
- Detected and removed duplicate records.
- Standardized inconsistent categorical values.
- Removed unwanted currency symbols and commas from charge-related columns.
- Converted columns into appropriate data types.
- Converted the signup date column into datetime format.
- Removed an unnecessary column.

### 3. Outlier Detection
- Used the Interquartile Range (IQR) method to identify potential outliers in selected numerical columns.
- Inspected the detected values and retained potential outliers that could represent valid customer records.

### 4. Data Transformation
- Created a `tenure_group` column to categorize customers based on their tenure.
- Extracted signup year and signup month from the signup date.
- Used grouping and pivot table operations to organize the data for further analysis.

### 5. Cleaned Dataset
The cleaned dataset is available in both CSV and Excel formats inside the `cleaned_data` folder.

## Project Status

**Completed**
- Data loading and initial inspection
- Missing value handling
- Duplicate detection and removal
- Categorical data standardization
- Data type conversion
- Outlier detection and inspection
- Feature creation and data transformation
- Exporting cleaned data in CSV and Excel formats

**Upcoming**
- Exploratory Data Analysis (EDA)
- Data visualization
- Churn pattern analysis
- Identification of key churn factors
- Business insights and recommendations

## Conclusion

The data cleaning, preprocessing, and transformation stages have prepared the telecom customer dataset for further exploratory analysis and churn-related insights.

## Author

**Akshaya S**  
B.Sc. Computer Science Graduate | Entry-Level Data Analyst
