

# LeetCode - Introduction to Pandas

## 📌 Problem Statement

This repository serves as an introduction to **Pandas**, which is a powerful data manipulation and analysis library for Python. It provides data structures like `DataFrame` and `Series`, designed to handle and manipulate large datasets efficiently. Pandas is widely used in data science and machine learning for tasks like data cleaning, exploration, and visualization.

This repository contains solutions to various **LeetCode** problems, where we use **Pandas** to manipulate and solve problems more effectively, especially those dealing with large datasets and structured data.

---

## 📊 Table of Contents

1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Pandas Basics](#pandas-basics)
4. [Pandas CheetSheet](#pandas-cheetSheet)
5. [LeetCode Problems](#leetcode-problems)
    - Problem 1: [Problem Title](#problem-1)
    - Problem 2: [Problem Title](#problem-2)
6. [Useful Links](#useful-links)

---

## 📚 Introduction

### What is Pandas?

**Pandas** is an open-source data manipulation and analysis library for Python. It offers data structures like `Series` (for one-dimensional data) and `DataFrame` (for two-dimensional data) that make it easy to manipulate, analyze, and visualize data in various formats (CSV, Excel, SQL databases, JSON, etc.).

#### Key Features:
- **Data Structures:** Pandas primarily offers two data structures:
  - `Series`: A one-dimensional labeled array, similar to a list or array.
  - `DataFrame`: A two-dimensional labeled data structure, like a table or spreadsheet, where each column can be a different type.
  
- **Data Alignment:** Automatically aligns data based on labels or indexes during operations.
- **Handling Missing Data:** Pandas provides methods to handle missing data in datasets.
- **Data Aggregation:** Allows you to group data and perform operations like sum, mean, count, etc.
- **Merging and Joining:** Easily combine different datasets using joins or merges.
- **Filtering and Sorting:** Provides rich functionality for filtering and sorting data based on multiple conditions.
  
#### Why Use Pandas?

- **Efficiency:** Pandas is optimized for performance and can handle large datasets much faster than traditional Python data structures.
- **Easy to Use:** With just a few lines of code, you can manipulate and analyze data easily.
- **Integration:** It integrates well with other libraries such as NumPy, Matplotlib, and Scikit-learn, making it ideal for data science and machine learning workflows.

---

## 🛠 Installation

To get started with Pandas, you need to install the library using the following command:

```bash
pip install pandas
```

Additionally, you might also need other dependencies, such as `numpy`, which Pandas relies on for numerical computations:

```bash
pip install numpy
```

---

## 🧑‍💻 Pandas Basics

Here are some fundamental Pandas operations you'll use to solve problems in this repository.

### 1. Importing Pandas

```python
import pandas as pd
```

### 2. Creating a DataFrame

A `DataFrame` is the core data structure in Pandas, and it can be created from various data sources like lists, dictionaries, or external files.

```python
# Creating a DataFrame from a dictionary
data = {'Name': ['John', 'Anna', 'Peter', 'Linda'],
        'Age': [28, 24, 35, 32]}
df = pd.DataFrame(data)
```

### 3. Data Inspection

- **View the first few rows**:
  ```python
  print(df.head())
  ```

- **Get DataFrame info**:
  ```python
  print(df.info())
  ```

- **Descriptive statistics**:
  ```python
  print(df.describe())
  ```

### 4. Selecting Data

- **Select a single column**:
  ```python
  df['Name']
  ```

- **Select multiple columns**:
  ```python
  df[['Name', 'Age']]
  ```

- **Row selection by index**:
  ```python
  df.iloc[0]  # Selects the first row
  ```

### 5. Data Cleaning

- **Handling missing values**:
  ```python
  df.isna().sum()  # Check for missing values
  df.dropna()  # Drop rows with missing values
  df.fillna(value=0)  # Replace NaN with a specific value
  ```

### 6. Grouping and Aggregation

- **Group by a column**:
  ```python
  df.groupby('Age').mean()  # Group by 'Age' and calculate the mean
  ```

### 7. Merging DataFrames

- **Merge two DataFrames**:
  ```python
  df1.merge(df2, on='column_name')
  ```

---
# 🧩 Pandas CheetSheet

<img src="Pandas CheetSheet\Pandas_Cheat_Sheet-1,Pandas_Cheat_Sheet-2\Pandas_Cheat_Sheet-1.svg" alt="cheet sheet">
<img src="Pandas CheetSheet\Pandas_Cheat_Sheet-1,Pandas_Cheat_Sheet-2\Pandas_Cheat_Sheet-2.svg">
---

## 🧩 LeetCode Problems

This repository includes solutions to various **LeetCode** problems using Pandas. Below are some examples:

### Problem 1: [Problem Title](#)
- **Description:** [Brief description of the problem]
- **Solution:**
  ```python
  # Pandas solution code
  ```

### Problem 2: [Problem Title](#)
- **Description:** [Brief description of the problem]
- **Solution:**
  ```python
  # Pandas solution code
  ```

Feel free to explore the other problems and their solutions in the `solutions/` folder.

---

## 🔗 Useful Links
- [Pandas Official Documentation](https://pandas.pydata.org/)
- [LeetCode](https://leetcode.com/)
- [Python Documentation](https://docs.python.org/3/)
- [Pandas Cheat Sheet](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)
- [Kaggle: Pandas Tutorials](https://www.kaggle.com/learn/pandas)
```
