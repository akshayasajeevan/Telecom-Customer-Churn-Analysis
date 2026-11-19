# Telecom Customer Churn Analysis

## 📌 Project Overview

Telecom Customer Churn Analysis is a Python-based data analytics project focused on understanding customer behavior and identifying patterns associated with customer churn.

The project covers data cleaning, preprocessing, feature transformation, exploratory data analysis (EDA), and data visualization. It explores customer information such as tenure, contract type, payment method, internet service, and charges to identify factors associated with customer retention.

The goal is to generate meaningful insights and business recommendations that can help improve customer retention.

## 🎯 Project Objectives

- Analyze telecom customer data and understand customer behavior.
- Identify customer churn patterns.
- Explore factors associated with customer retention.
- Analyze churn based on contract type, payment method, internet service, and tenure.
- Examine customer signup trends.
- Generate business insights and recommendations to help reduce customer churn.

## 🛠️ Tools & Technologies

| Tool             | Purpose                        |
| ---------------- | ------------------------------ |
| Python           | Data analysis                  |
| Jupyter Notebook | Development and analysis       |
| Pandas           | Data cleaning and manipulation |
| NumPy            | Numerical operations           |
| Matplotlib       | Data visualization             |
| Seaborn          | Statistical visualization      |
| CSV & Excel      | Data storage and handling      |

## 📂 Project Structure

```text
Telecom-Customer-Churn-Analysis/
│
├── cleaned_data/
│   ├── telecom_churn_cleaned_csv.csv
│   └── telecom_churn_cleaned_excel.xlsx
│
├── data/
│   ├── Telecom Churn raw csv.csv
│   └── Telecom Churn raw excel.xlsx
│
├── images/
│   ├── Churn Distribution.png
│   ├── Churn Rate by Payment Method.png
│   ├── Churn by Contract Type.png
│   ├── Churn by Internet Service.png
│   ├── Customer Signup Trend.png
│   ├── Monthly Charges Distribution.png
│   ├── Monthly Charges vs Churn.png
│   ├── Numerical Feature Correlation.png
│   ├── Tenure Distribution.png
│   └── Tenure vs Churn.png
│
├── Telecom Customer Churn Analysis.ipynb
├── requirements.txt
└── README.md
```

## 📁 Dataset Information

The dataset contains telecom customer information, including:

- Customer details
- Internet and service information
- Contract types and payment methods
- Customer tenure
- Monthly and total charges
- Signup dates
- Customer churn status

Both raw and cleaned datasets are available in CSV and Excel formats.

## 🔄 Project Workflow

### 1. Data Loading & Inspection

- Loaded the dataset using Pandas.
- Examined the dataset shape, column names, and data types.
- Reviewed descriptive statistics.
- Checked for missing values and duplicate records.

### 2. Data Cleaning & Preprocessing

- Handled selected numerical missing values using median imputation.
- Identified and removed duplicate records.
- Standardized inconsistent categorical values.
- Removed unwanted currency symbols and commas from charge-related columns.
- Converted columns into appropriate data types.
- Converted signup dates into datetime format.
- Removed an unnecessary column.

### 3. Outlier Detection & Handling

- Used the Interquartile Range (IQR) method to identify potential outliers in selected numerical columns.
- Applied IQR-based filtering to the `tenure` and `monthly_charges` columns.
- Removed records that fell outside the calculated lower and upper limits for these columns.

### 4. Data Transformation

- Created a `tenure_group` column to categorize customers based on tenure.
- Extracted signup year and signup month from the signup date.
- Used grouping and pivot table operations to organize data for analysis.

### 5. Exploratory Data Analysis (EDA)

- Analyzed overall customer churn distribution.
- Examined churn across different contract types.
- Compared churn patterns across payment methods and internet services.
- Analyzed customer signup trends by year and month.
- Explored monthly charges and customer tenure.
- Studied relationships between numerical features and churn.

### 6. Data Visualization

Created 10 visualizations using Matplotlib and Seaborn to understand customer behavior and identify important churn patterns.

## 📈 Key Findings & Insights

- The dataset contains **19,712 customers**, of which **1,571 customers (7.97%)** have churned.
- Customer signup numbers were highest in 2023 among the analyzed years.
- The highest churn rate by signup year was observed in 2024 (8.47%).
- August recorded the highest monthly churn rate (9.41%).
- The two-year contract group had the highest churn rate among contract types (8.15%), although differences were small.
- Fiber optic customers showed a slightly higher churn rate (8.07%) than DSL customers (7.85%).
- Electronic check payments accounted for 45.1% of all churned customers.
- Established customers showed the highest churn rate among the analyzed tenure groups (8.78%).
- Churned and retained customers had the same median monthly charges (70.18).

*Note: These findings describe patterns in the analyzed dataset and do not establish cause-and-effect relationships.*

## 💡 Business Recommendations

Based on the analysis, the following recommendations may help improve customer retention:

- **Customer Engagement:** Introduce personalized offers and regular customer engagement activities.
- **Payment Experience:** Review the electronic check payment experience and identify possible customer concerns.
- **Service Quality:** Monitor internet service quality and customer satisfaction.
- **Customer Retention:** Strengthen customer relationships through suitable retention strategies.
- **Pricing Strategy:** Review pricing plans and provide suitable options based on customer needs.
- **Continuous Monitoring:** Perform regular churn analysis to identify changes in customer behavior.

## 📊 Visualizations

The project includes 10 visualizations. Three selected visualizations are presented below.

### 1. Customer Signup Trend

Shows how customer signups changed over time.



### 2. Churn by Contract Type

Compares customer churn across different contract types.



### 3. Monthly Charges vs Churn

A violin plot comparing the distribution of monthly charges among churned and retained customers.



*The remaining visualizations are available in the `images/` folder.*

## ⚙️ Installation & Requirements

**1. Clone the repository**

```bash
git clone https://github.com/akshayasajeevan/Telecom-Customer-Churn-Analysis.git
```

**2. Navigate to the project folder**

```bash
cd Telecom-Customer-Churn-Analysis
```

**3. Install the required libraries**

```bash
pip install -r requirements.txt
```

**4. Open Jupyter Notebook**

```bash
jupyter notebook
```

## 📝 Conclusion

This project provided practical experience in data cleaning, preprocessing, feature transformation, exploratory data analysis, and data visualization using Python.

The analysis helped identify customer churn patterns and explore factors associated with customer retention. The findings and recommendations provide useful insights that may support better customer engagement and retention strategies.

## 👩‍💻 Author

**Akshaya S**
B.Sc. Computer Science Graduate | Entry-Level Data Analyst

- **GitHub:** [akshayasajeevan](https://github.com/akshayasajeevan)
