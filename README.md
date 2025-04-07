# Task1DSINTERN
# 🧼 Mall Customer Segmentation Data Cleaning

This project is part of a **Data Analyst Internship Task** that involves data cleaning and preprocessing of the **Mall Customer Segmentation Dataset** using Python and Pandas.

---

## 📁 Dataset Description

The dataset contains information about customers in a mall, including:

- `CustomerID`: Unique ID assigned to each customer
- `Gender`: Male or Female
- `Age`: Age of the customer
- `Annual Income (k$)`: Annual income in thousands of dollars
- `Spending Score (1-100)`: Score assigned based on customer behavior and spending nature

---

## 🧪 Tools & Technologies Used

- **Python** (v3+)
- **Pandas** (for data manipulation)
- Jupyter Notebook / Google Colab

---

## 🔍 Tasks Performed

### 1. **Importing the Dataset**
- Used `pandas.read_csv()` to load the dataset into a DataFrame.

### 2. **Initial Inspection**
- Used `.info()` and `.isnull().sum()` to check for data types and missing values.

### 3. **Handling Missing Values**
- All rows with missing values were dropped using `df.dropna()` (for simplicity and safety).

### 4. **Removing Duplicates**
- Duplicate rows were identified and removed using `df.drop_duplicates()`.

### 5. **Standardizing Column Names**
- Column names were converted to lowercase and spaces replaced with underscores for consistency.
  - Example: `Annual Income (k$)` → `annual_income_(k$)`

### 6. **Cleaning Gender Column**
- Standardized all gender values (e.g., "male", "Male") to have consistent formatting using `.str.capitalize()`.

### 7. **Fixing Data Types**
- Converted:
  - `CustomerID` to **string**
  - `Age` to **integer**

### 8. **Exporting Cleaned Data**
- The cleaned dataset was exported to a new CSV file named:  
  ✅ `cleaned_mall_customers.csv`

---

## 📦 Output Files

- `cleaned_mall_customers.csv` → Final cleaned dataset
- `data_cleaning_script.py` or `.ipynb` → Python code used for cleaning

---

## ✅ Conclusion

All major data quality issues such as **null values**, **duplicate records**, **inconsistent formatting**, and **data types** were handled. The dataset is now clean, consistent, and ready for analysis or modeling.

---

## 🔗 Dataset Source

You can find the original dataset here:  
**[Mall Customer Segmentation Data on Kaggle](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)**
