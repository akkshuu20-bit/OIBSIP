# Task 3 - Data Cleaning

## Objective

The objective of this task is to clean and prepare a messy retail sales dataset for further analysis. The cleaning process includes handling missing values, checking duplicates, correcting data types, detecting outliers, normalization, and feature engineering.

## Dataset

The dataset used for this task is `retail_store_sales.csv`.

The dataset contains retail transaction information such as transaction ID, customer ID, category, item, price per unit, quantity, total spent, payment method, location, transaction date, and discount information.

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

### 2. Handling Missing Values

Missing values were identified in columns such as:

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

Potential outliers were found in `Total Spent`. These values were retained because they may represent genuine high-value retail transactions.

### 6. Normalization

Min-Max normalization was applied to numerical variables:

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

## Final Dataset

After cleaning and feature engineering:

- Total Records: 12,575
- Total Columns: 18
- Missing Values: 0
- Duplicate Rows: 0

The cleaned dataset was saved as:

`retail_store_sales_cleaned.csv`

## Files

- `Task_3_Data_Cleaning.ipynb` - Data cleaning and analysis notebook
- `retail_store_sales_cleaned.csv` - Cleaned and analysis-ready dataset
- `README.md` - Project documentation

## Conclusion

The messy retail sales dataset was successfully cleaned and transformed into a structured, analysis-ready dataset. Missing values were handled, duplicate records were checked, data types were corrected, potential outliers were analyzed, numerical data was normalized, and useful features were created.

The final dataset contains 12,575 records and 18 columns with zero missing values and zero duplicate records.
