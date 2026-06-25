# Day 2 - Pandas and NumPy Fundamentals

## 1. Pandas

Pandas is a Python library used for data manipulation and analysis.

Import:

import pandas as pd

---

## 2. DataFrame

A DataFrame is a 2D tabular structure consisting of rows and columns.

Example:

| Name | Age |
|------|-----|
| John | 20 |

---

## 3. Why pd?

Instead of writing:

pandas.DataFrame()

we write:

pd.DataFrame()

for convenience.

---

## 4. NumPy

NumPy is a Python library for numerical computing.

Import:

import numpy as np

---

## 5. NumPy Arrays

Arrays are similar to lists but faster and optimized for numerical operations.

Example:

np.array([1,2,3])

---

## 6. Difference Between Pandas and NumPy

NumPy:
- Numerical calculations
- Arrays
- Faster mathematical operations

Pandas:
- Data manipulation
- Tables/DataFrames
- Data analysis

---

## 7. Iris Dataset in Pandas

Converted dataset into a DataFrame to view data in tabular form.

Useful methods:

df.head()

df.tail()

df.shape()

df.columns