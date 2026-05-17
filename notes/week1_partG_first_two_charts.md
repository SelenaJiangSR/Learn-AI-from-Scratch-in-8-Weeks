# Week 1 Part G — First Two Charts

## What I Learned in This Part

In this part, I created my first two simple charts in Python using Matplotlib.

My goal was to learn how to turn a small dataset into visual form and explain what the charts show.

The two charts I created were:

- a histogram of scores
- a bar chart of student names and scores

This part helped me understand that visualization is an important way to explore and communicate data.

---

# Why This Part Matters

Charts make data easier to understand.

Instead of only reading rows and columns, I can use charts to see patterns more clearly.

For example, charts can help me answer questions such as:

- How are values distributed?
- Which student has the highest score?
- Are there big differences between values?
- What does the data look like visually?

This part helped me move from reading data to visualizing data.

---

# Step-by-Step Practice

## Step 1 — Import the required libraries

```python
import pandas as pd
import matplotlib.pyplot as plt
```

This imports Pandas for reading the CSV file and Matplotlib for creating charts.

---

## Step 2 — Read the dataset

```python
df = pd.read_csv("students.csv")
```

This loads the student dataset into a DataFrame.

---

## Step 3 — Create a histogram of scores

```python
plt.hist(df["score"])
plt.title("Distribution of Scores")
plt.xlabel("Score")
plt.ylabel("Frequency")
plt.show()
```

### What this step taught me

A histogram helps show how numerical values are distributed.

---

## Step 4 — Create a bar chart of names and scores

```python
plt.bar(df["name"], df["score"])
plt.title("Student Scores")
plt.xlabel("Student Name")
plt.ylabel("Score")
plt.show()
```

### What this step taught me

A bar chart helps compare values across different categories.

---

# Full Code Example

```python
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("students.csv")

# Histogram of scores
plt.hist(df["score"])
plt.title("Distribution of Scores")
plt.xlabel("Score")
plt.ylabel("Frequency")
plt.show()

# Bar chart of student scores
plt.bar(df["name"], df["score"])
plt.title("Student Scores")
plt.xlabel("Student Name")
plt.ylabel("Score")
plt.show()
```

---

# My Practice Result

From this practice, I created two beginner-level charts from my student dataset.

---

## Chart 1 — Histogram of Scores

This chart used the score column.

- x-axis = score values
- y-axis = frequency

### What the chart shows

The histogram shows how the score values are distributed in the dataset.

Since the dataset is very small, the chart is simple, but it still helped me understand how scores are spread out.

---

## Chart 2 — Bar Chart of Student Scores

This chart used:

- name on the x-axis
- score on the y-axis

- x-axis = student names
- y-axis = scores

### What the chart shows

The bar chart makes it easy to compare the scores of different students.

From this chart, I can quickly see which student has the highest score and which student has the lowest score.

---

# What I Understand Now

From this part, I understand that charts are a useful way to explore and communicate data.

I also understand that:

- a histogram is useful for showing the distribution of one numeric variable
- a bar chart is useful for comparing values across categories
- labels and titles are important because they make charts easier to understand

This part helped me connect Python code with visual output.

---

# Reflection

This part was my first experience turning a dataset into charts.

Before this, I was only looking at data in rows, columns, and summary statistics.

Now I can also look at data visually.

Even though the dataset is very small, this part helped me build the habit of explaining charts clearly:

- what is on the x-axis
- what is on the y-axis
- what the chart is showing

I think this is an important beginner skill for future data analysis and AI-related work.

---

# Files Created in This Part

```text
students.csv
partG_first_two_charts.py
notes/week1_partG_first_two_charts.md
```

---

# Today's Workflow

1. Create a Python file:

```text
partG_first_two_charts.py
```

2. Copy the Full Code Example into the file

3. Run the Python script

4. View the two charts

5. Take screenshots of both charts

6. Upload the screenshots to GitHub

7. Paste this markdown note into:

```text
notes/week1_partG_first_two_charts.md
```

---

# Key Beginner Concepts I Practiced

| Concept | Meaning |
|---|---|
| Data Visualization | Turning data into charts or graphs |
| Histogram | A chart showing the distribution of numeric values |
| Bar Chart | A chart comparing categories and values |
| x-axis | Horizontal axis |
| y-axis | Vertical axis |
| Frequency | How often values appear |
| Matplotlib | A Python library for visualization |
| DataFrame | A table-like data structure in Pandas |

---

# Final Reflection

This was my first step into data visualization using Python.

I learned how to:

- read a dataset
- create charts
- label axes and titles
- explain visual output
- connect data with visual understanding

This part helped me understand that visualization is one of the core skills in data analysis and AI.

Even simple charts can help reveal useful information from data.
