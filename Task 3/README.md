# Task 3 - Data Cleaning

## Objective

The objective of this task is to clean and prepare a messy retail sales dataset for further analysis. The cleaning process includes handling missing values, checking duplicates, correcting data types, detecting outliers, normalization, and feature engineering.

## Dataset

The original dataset used for this task is `retail_store_sales task 3.csv`.

The dataset contains retail transaction information such as:

- Transaction ID
- Customer ID
- Category
- Item
- Price Per Unit
- Quantity
- Total Spent
- Payment Method
- Location
- Transaction Date
- Discount Applied

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

## Data Cleaning Steps

### 1. Data Inspection

The dataset was inspected to understand its structure, columns, data types, and missing values.

The original dataset contained:

- 12,575 records
- 11 columns

### 2. Handling Missing Values

Missing values were identified in the following columns:

- Item
- Price Per Unit
- Quantity
- Total Spent
- Discount Applied

Missing values were handled using appropriate methods such as mode and median imputation.

### 3. Duplicate Records

Duplicate records were checked using Pandas.

No duplicate rows were found in the dataset.

### 4. Data Type Correction

The `Transaction Date` column was converted from object format to datetime format for accurate date-based analysis.

### 5. Outlier Detection

The Interquartile Range (IQR) method was used to detect potential outliers in numerical columns.

Potential outliers were found in the `Total Spent` column. These values were retained because they may represent genuine high-value retail transactions.

### 6. Normalization

Min-Max normalization was applied to the following numerical variables:

- Price Per Unit
- Quantity
- Total Spent

The original values were preserved, and normalized values were stored in separate columns.

### 7. Feature Engineering

The following new features were created:

- `Year`
- `Month`
- `Day`
- `Amount_Per_Item`

These features make the dataset more useful for further analysis.

## Before and After Cleaning

### Before Cleaning

- Records: 12,575
- Columns: 11
- Missing values: Present
- Duplicate records: 0
- Transaction Date: Object data type

### After Cleaning

- Records: 12,575
- Columns: 18
- Missing values: 0
- Duplicate records: 0
- Transaction Date: Datetime format
- Additional features: Year, Month, Day, Amount_Per_Item
- Normalized features: Added

## Final Dataset

The cleaned dataset was saved as:

`retail_store_sales_cleaned.csv`

The final dataset contains:

- 12,575 records
- 18 columns
- 0 missing values
- 0 duplicate records

## Files

- `Cleaning_Data_task_3.ipynb` - Data cleaning and analysis notebook
- `retail_store_sales task 3.csv` - Original messy dataset
- `retail_store_sales_cleaned.csv` - Cleaned and analysis-ready dataset
- `README.md` - Project documentation

## Conclusion

The messy retail sales dataset was successfully cleaned and transformed into a structured, analysis-ready dataset. Missing values were handled, duplicate records were checked, data types were corrected, potential outliers were analyzed, numerical data was normalized, and useful features were created.

The final dataset contains 12,575 records and 18 columns with zero missing values and zero duplicate records.

The cleaned dataset can now be used for further data analysis and visualization.
