# Week 1 Part D — Python Data Tools

## NumPy

NumPy is a Python library mainly used for arrays and numerical computing.

Example:
- storing numbers in arrays
- performing mathematical operations on arrays
- calculating averages or sums

Basic usage:
```python
import numpy as np

arr = np.array([1, 2, 3, 4])
print(arr)
print(arr + 10)
print(arr * 2)
print(np.mean(arr))
print(np.sum(arr))

---

## Pandas

Pandas is a Python library mainly used for tabular and structured data.

Example:
- reading a CSV file
- checking column names
- viewing the first few rows of a dataset

My understanding:
Pandas is one of the most useful tools for working with table-like data in Python.

---

## Matplotlib

Matplotlib is a Python library mainly used for plotting and data visualization.

Example:
- drawing a histogram
- creating a scatter plot
- making a bar chart

My understanding:
Matplotlib helps turn data into charts so I can understand it more clearly.

---

## Relationship Between the Three Tools

These tools are often used together in data work.

Example workflow:
1. Use Pandas to read a CSV file
2. Use NumPy for numerical operations
3. Use Matplotlib to visualize the data

   

My understanding:
NumPy handles numbers, Pandas handles tables, and Matplotlib helps visualize the results.
