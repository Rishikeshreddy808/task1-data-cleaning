# Task 1 — Data Cleaning & Preprocessing (Coffee Sales Dataset)

## 📌 Objective
Clean and preprocess a raw coffee sales dataset by handling data types, duplicates, text standardization, and preparing the dataset for further analysis.

## 📂 Dataset
- **Raw file:** `coffe.csv`
- **Rows:** 3,547
- **Columns:** 11  
  (`hour_of_day`, `cash_type`, `money`, `coffee_name`, `Time_of_Day`, `Weekday`, `Month_name`, `Weekdaysort`, `Monthsort`, `Date`, `Time`)

## ⚙️ Steps Performed
1. **Standardized column names** → converted to lowercase, snake_case format.
2. **Converted data types**:
   - `money` → numeric (float).
   - `date` & `time` → converted into proper datetime.
   - Created a new `datetime` column by combining date & time.
3. **Text cleaning**:
   - Standardized `coffee_name`, `cash_type`, and `time_of_day` for consistency.
4. **Removed duplicates** → dropped exact duplicate rows.
5. **Handled outliers** → removed transactions with negative or unrealistic money values.
6. **Dropped redundant columns** → e.g., `time` after creating combined datetime.
7. **Exported cleaned dataset** → saved as `cleaned_coffee.csv`.

## ✅ Deliverables
- **Raw dataset:** `coffe.csv`
- **Cleaned dataset:** `cleaned_coffee.csv`
- **Notebook:** `Task1_DataCleaning.ipynb`

## 📊 Key Insights
- The dataset was already free of missing values.
- Main issues were inconsistent text formatting and unoptimized column types.
- After cleaning, the dataset is ready for **Task 2 (Visualization)** and **Task 3 (Dashboard Design)**.

