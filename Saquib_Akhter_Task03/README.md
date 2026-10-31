# OIBSIP Task 3: Data Cleaning and Preprocessing

## Project Overview

This project focuses on cleaning and preprocessing a real-world retail store sales dataset using Python and its data analysis libraries.

The objective is to identify data quality issues, handle missing values, investigate duplicates and outliers, standardise data, correct data types, and export a cleaned dataset for further analysis.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset Information

**Dataset:** Retail Store Sales

The dataset contains retail transaction information, including:

- Transaction ID
- Customer ID
- Product Category
- Item
- Price Per Unit
- Quantity
- Total Spent
- Payment Method
- Location
- Transaction Date
- Discount Applied

**Original dataset dimensions:** 12,575 rows and 11 columns.

## Project Workflow

### 1. Data Loading and Exploration
- Loaded the raw CSV dataset using Pandas.
- Examined dataset dimensions, column names, and data types.
- Generated an initial data quality report.

### 2. Data Quality Assessment
- Identified missing values.
- Checked duplicate records.
- Investigated numerical ranges and date validity.
- Checked the relationship between price, quantity, and total spending.

### 3. Missing Value Treatment
- Replaced missing item names with `Unknown`.
- Used median imputation for missing numerical values.
- Preserved unknown discount statuses as missing rather than assuming they were false.

### 4. Duplicate Removal and Standardisation
- Checked and removed duplicate records where present.
- Removed unnecessary whitespace from text fields.
- Standardised categorical text formatting.
- Converted transaction dates, numeric fields, and discount status to appropriate data types.

### 5. Outlier Investigation
- Used the Interquartile Range (IQR) method.
- Investigated unusually high transaction values.
- Retained potentially valid transactions instead of automatically deleting them.

### 6. Quality Comparison
- Compared the original and cleaned datasets.
- Generated before-and-after quality reports.
- Documented missing-value handling decisions.

### 7. Export
- Exported the cleaned dataset to CSV format.
- Verified the exported dataset.

## Important Data Cleaning Decisions

| Issue | Action |
|---|---|
| Missing Item | Replaced with `Unknown` |
| Missing Price Per Unit | Median imputation |
| Missing Quantity | Median imputation |
| Missing Total Spent | Median imputation |
| Missing Discount Applied | Retained as unknown |
| Duplicate records | Checked; none found |
| Potential outliers | Investigated and retained when considered valid |
| Inconsistent text formatting | Standardised |
| Incorrect data types | Converted to appropriate types |

**Note:** Median-imputed numerical values are estimates, not original transaction values. The unknown discount statuses are intentionally preserved.

## Project Structure

```text
TASK03/
│
├── data/
│   ├── raw/
│   │   └── retail_store_sales.csv
│   │
│   └── cleaned/
│       └── retail_store_sales_cleaned.csv
│
├── outputs/
│   ├── initial_data_quality_report.csv
│   ├── before_after_comparison.csv
│   └── missing_values_comparison.csv
│
├── screenshots/
│
├── data_cleaning.ipynb
├── requirements.txt
└── README.md
```

## How to Run the Project

1. Clone or download this repository.
2. Open the project folder in VS Code.
3. Create and activate a virtual environment.
4. Install dependencies:

```bash
pip install -r requirements.txt
```

5. Open the notebook:

```bash
jupyter notebook
```

6. Run `data_cleaning.ipynb` from beginning to end.

## Learning Outcomes

- Practical experience with data cleaning and preprocessing.
- Identifying and handling missing values.
- Detecting duplicate records and outliers.
- Data type conversion and text standardisation.
- Creating data quality reports.
- Exporting clean datasets for further analysis.

## Author

**Saquib Akhter**

GitHub: [@iamsaqb](https://github.com/iamsaqb)

Project: OIBSIP Data Analytics Internship, Task 3.