# Task 1: Data Cleaning and Preprocessing

## 📊 Project Overview
This project demonstrates comprehensive data cleaning and preprocessing techniques applied to the Mall Customer Segmentation dataset from Kaggle. The goal is to transform raw, messy data into a clean, analysis-ready dataset.

## 🎯 Objective
Clean and prepare a raw dataset containing null values, duplicates, and inconsistent formats using Python and Pandas.

## 📁 Dataset
**Mall Customer Segmentation Data** from Kaggle
- **Source**: [Kaggle Mall Customer Segmentation](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Original File**: `mall_customers.csv`
- **Cleaned File**: `mall_customers_cleaned.csv`

## 🛠️ Tools Used
- **Python 3.x**
- **Pandas** - Data manipulation
- **NumPy** - Numerical operations
- **Jupyter Notebook** - Interactive analysis

## 📋 Data Cleaning Steps Performed

### 1. Initial Data Assessment
- Loaded and inspected dataset structure
- Identified missing values, duplicates, and data types
- Generated summary statistics

### 2. Column Name Standardization
- Converted to lowercase
- Replaced spaces with underscores
- **Example**: `CustomerID` → `customer_id`, `Annual Income (k$)` → `annual_income_k`

### 3. Missing Value Treatment
- Numerical columns: Filled with median values
- Categorical columns: Filled with mode values
- Comprehensive missing value analysis

### 4. Duplicate Handling
- Identified and removed duplicate rows
- Preserved data integrity

### 5. Data Type Correction
- Ensured proper data types for each column
- Converted categorical variables to appropriate formats

### 6. Text Standardization
- Standardized gender values to consistent format
- Removed whitespace and case inconsistencies

### 7. Outlier Treatment
- Used IQR method to detect outliers
- Capped extreme values to reduce skewness

### 8. Feature Engineering
- Created age groups for better segmentation
- Enhanced dataset for analytical purposes

## 📊 Dataset Description

### Original Dataset Columns:
- `CustomerID` - Unique customer identifier
- `Gender` - Customer gender (Male/Female)
- `Age` - Customer age in years
- `Annual Income (k$)` - Annual income in thousands
- `Spending Score (1-100)` - Mall spending score

### New Columns Added:
- `age_group` - Categorical age ranges for segmentation

## 🚀 How to Run

### Prerequisites
```bash
pip install -r scripts/requirements.txt
