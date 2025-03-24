# aviation-analysis-project
A data-driven exploration of aircraft accident data from 1962 to 2023, using Python and Tableau to assess risk factors, trends, and safety insights. This project involves data cleaning, exploratory analysis, and interactive visualization to uncover patterns in aviation safety.

## **Data Loading**
### **Importing the Dataset for Analysis**  

The first step in any data analysis process is loading the dataset into the environment. 
This allows us to inspect, clean, and prepare the data for further exploration.  

### **1. Importing Necessary Libraries**  
Before loading the dataset, we imported essential Python libraries for data manipulation and analysis:  
```python
import pandas as pd  # For data handling
import numpy as np   # For numerical operations
import matplotlib.pyplot as plt  # For visualizations
import seaborn as sns  # For advanced visualization
```


### **2. Reading the Dataset**  
The aviation accident dataset is loaded using **Pandas**:  
```python
aviation_df = pd.read_csv("aviation_accidents.csv")  # Replace with actual file path
```


### **3.  Inspecting the Data**  
After loading, initial checks are performed to understand the dataset structure:  

- **View first few rows:**  
  ```python
  aviation_df.head()
  ```
- **Check dataset shape (rows, columns):**  
  ```python
  aviation_df.shape
  ```
- **Get column names and data types:**  
  ```python
  aviation_df.info()
  ```
- **Check summary statistics:**  
  ```python
  aviation_df.describe()
  ```
  

### **4. Verifying Data Integrity**  
To ensure data integrity, we checked for:  
- **Duplicate values** – using `.duplicated().sum()`
- **Inconsistent column names** – using `aviation_df.columns`  
- **Missing values** – using `.isnull().sum()`  


### **Outcome: A Successfully Loaded Dataset**  
With the data now loaded and verified, we proceeded with **cleaning and preprocessing** to prepare it for analysis.


## Data Cleaning
### **Preparing the Dataset for Analysis**  

Data cleaning is a crucial step in the data analysis process. It ensures the dataset is accurate, consistent, and ready for further analysis. Below are the key steps performed to clean our aviation accident dataset:  

### **1. Handling Missing Values**  
Missing values can affect the reliability of our analysis. Different strategies have been used to handle them:  

- **Numerical Data:** Filled missing values with the mean or median, rounding up to the nearest whole number.  
- **Categorical Data:** Filled missing values with the most frequent value (mode).  
- **Columns with High Missing Percentages:** Considered removing features with excessive missing data that provided little value.  


### **2. Standardizing Column Names**  
To ensure consistency in the dataset, the following has been done:  
- Capitalizing the first letter of every word in column names.  


### **3. Handling Duplicate Data**  
- Checked for duplicate records to avoid biased results.  
- Verified that the dataset contained no duplicate values before proceeding.  


### **4. Adding New Features for Better Insights**  
- New features were added to enhance the analysis.  


### **Outcome: A Clean & Structured Dataset**  
After these steps, the dataset is now:  
- Free of missing values.  
- Consistent in format.  
- Enhanced with new features for deeper analysis.  
