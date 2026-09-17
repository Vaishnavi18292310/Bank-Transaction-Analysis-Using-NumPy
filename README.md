# Bank Transaction Analysis Using NumPy

## 📌 Project Overview

This project focuses on analyzing a **50,000-record bank transaction dataset** using Python and NumPy.

The objective was to apply NumPy concepts to real-world transaction data and generate meaningful insights related to transaction amounts, customer demographics, account balances, transaction channels, login attempts, and transaction behavior.

The project was designed as a hands-on NumPy data analysis project with a focus on practical **Data Analyst and Data Engineering** use cases.

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Jupyter Notebook

## 📊 Dataset

The dataset contains **50,000 bank transaction records** with 15 attributes, including:

* Transaction ID
* Account ID
* Transaction Amount
* Transaction Date
* Transaction Type
* Location
* Device ID
* IP Address
* Merchant ID
* Channel
* Customer Age
* Customer Occupation
* Transaction Duration
* Login Attempts
* Account Balance

> Note: The dataset does not contain an actual fraud-label column. Therefore, the project does not classify transactions as fraudulent. Instead, rule-based transaction indicators were created for analytical purposes.

## 🔍 Analysis Performed

### 1. Transaction Amount Analysis

* Calculated total transaction amount
* Calculated average transaction amount
* Identified minimum and maximum transaction values
* Calculated standard deviation
* Identified high-value transactions

### 2. Customer Age Analysis

* Calculated average customer age
* Identified minimum and maximum ages
* Counted customers above 60 years
* Calculated their percentage of total transactions

### 3. Login Attempt Analysis

* Identified minimum and maximum login attempts
* Calculated average login attempts
* Identified transactions with more than two login attempts

### 4. Account Balance Analysis

* Calculated average account balance
* Identified minimum and maximum balances
* Analyzed accounts based on balance thresholds

### 5. Transaction Behavior Analysis

* Applied multiple Boolean conditions
* Identified high-value transactions combined with higher login attempts
* Compared Debit and Credit transactions
* Analyzed transaction distribution across locations and channels

### 6. Customer Occupation Analysis

* Identified unique customer occupations
* Counted transactions by occupation
* Identified the occupation with the highest transaction activity
* Calculated its percentage of total transactions

### 7. Transaction Duration Analysis

* Calculated average transaction duration
* Identified minimum and maximum duration
* Identified transactions exceeding 100 seconds

### 8. Business Calculations

Applied NumPy vectorization and broadcasting to calculate:

* 2% transaction processing fees
* Final transaction amounts after fees

### 9. Transaction Categorization

Used `np.where()` to categorize transactions into:

* HIGH — transaction amount above 1000
* NORMAL — transaction amount 1000 or below

### 10. Missing-Value Analysis

Checked numerical columns for missing values using NumPy functions such as:

* `np.isnan()`
* `np.sum()`

## 🧠 NumPy Concepts Practiced

This project covers practical applications of:

* NumPy array creation
* Array properties: `ndim`, `shape`, `size`, `dtype`
* Indexing and slicing
* Boolean indexing
* Multiple conditions using `&` and `|`
* Aggregation functions
* `np.unique()`
* `np.argmax()`
* `reshape()`
* `flatten()`
* `ravel()`
* Transpose
* `vstack()` and `hstack()`
* `split()`
* Array modification
* `np.where()`
* Broadcasting
* Vectorization
* Missing-value handling
* Data type conversion using `astype()`

## 📈 Key Results

Some observations from the dataset:

* Total transactions analyzed: **50,000**
* Average transaction amount: **297.87**
* Transactions above 1,000: **1,788**
* Average customer age: **44.65**
* Customers above 60: **11,237**
* Average account balance: **5,122.74**
* Most-used transaction channel: **Branch**
* Most active occupation by transaction count: **Student**
* Transactions above 100 seconds: **27,903**

## 📂 Project Structure

```text
Bank-Transaction-NumPy-Analysis/
│
├── Bank_transactions_data.csv
├── NumPy_Bank_Transaction_Analysis.ipynb
└── README.md
```

## 🎯 Learning Outcome

Through this project, I strengthened my ability to use NumPy for practical data analysis, including **data extraction, filtering, aggregation, transformation, vectorized calculations, and business-oriented analysis**.

The project also provided hands-on experience working with a mixed-type financial transaction dataset and understanding how data types affect NumPy operations.

## 🚀 Future Scope

This project can be extended using:

* Pandas for advanced data cleaning and analysis
* Matplotlib/Seaborn for visualization
* SQL for transactional analysis
* Power BI for interactive dashboards
* PySpark for large-scale transaction processing
* Machine learning for fraud-risk modeling when a properly labeled fraud dataset is available
