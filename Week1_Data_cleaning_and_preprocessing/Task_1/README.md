# synent-task1-datacleaning-Hetvi-Patoliya
Data cleaning & preprocessing on Titanic dataset — handling missing values, duplicates, and type conversions | Synent Technologies Internship

# Titanic Data Cleaning & Preprocessing

## Problem Statement
The raw Titanic dataset contains missing values, irrelevant columns,
inconsistent data types and poorly named columns.
The goal is to clean and preprocess it to make it ready for analysis.

## Dataset
- **Source:** [Kaggle Titanic Dataset](https://www.kaggle.com/datasets/brendan45774/test-file)
- **Rows:** 1309
- **Columns:** 9 (after cleaning)

## Approach

### 1. Data Cleaning
- Dropped 18 irrelevant zero-filled columns (`zero.1` to `zero.18`)
- Handled 2 missing values in `Embarked` column using mode
- Renamed column `2urvived` to `Survived`

### 2. Preprocessing
- Converted `Age` from float to int
- Converted `Survived` to bool
- Mapped `Embarked` float codes to actual port names
- Dropped `Passengerid` as it is not useful for analysis
- Renamed `sibsp` → `Siblings_Spouses`, `Parch` → `Parents_Children`

## Results
- Clean dataset with no missing values
- Proper column names and data types
- Ready for EDA and modeling

## Tools Used
- Python
- Pandas
- Jupyter Notebook