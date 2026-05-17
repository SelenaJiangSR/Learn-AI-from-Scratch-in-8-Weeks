# Week 1 Part F — Basic Data Exploration

## What I Learned in This Part

In this part, I started doing basic exploration on a small dataset after successfully reading it with Pandas.

My goal was to answer simple questions such as:

- what the dataset is about
- what fields it contains
- which fields seem important
- whether there are missing values
- what one numeric column looks like statistically

This part helped me move from simply loading a dataset to actually beginning to understand it.

---

## What This Dataset Is About

This is a simple student dataset.

It contains basic information about students, including:

- name
- age
- score

My understanding:
This dataset is small, but it is useful for beginner practice because it is easy to inspect and understand.

---

## Fields in the Dataset

The dataset contains three columns:

- `name`
- `age`
- `score`

### What each field means

- `name` = the student's name
- `age` = the student's age
- `score` = the student's score

---

## Which Fields Seem More Important?

In this small dataset, the most important fields for exploration are:

- `age`
- `score`

These two columns are numeric, so they are more useful for statistics and charts.

The `name` column is still useful, but it mainly works as an identifier rather than a numeric feature for analysis.

---

## Step-by-Step Practice

Step 1 — Read the dataset

```python 
import pandas as pd

df = pd.read_csv("students.csv")
```
Step 2 — Preview the dataset

```print(df.head())```
This shows the first few rows of the dataset.
What this step taught me:
Looking at the first few rows helps me quickly understand what the data looks like.

Step 3 — Check the columns
```print(df.columns)```
This shows the column names.

What this step taught me:
Checking the columns helps me understand what fields are included in the dataset.

Step4 — Check the size of the dataset
```print(df.shape)```
This shows the number of rows and columns.

What this step taught me:
The shape tells me how large the dataset is.

Step 5 — Check missing values in one column
```print(df["score"].isnull().sum())```
This checks how many missing values are in the score column.

What this step taught me:
Checking missing values is a basic but important step in data exploration.

Step 6 — Check basic statistics for one numeric column
```print(df["score"].describe())```
This shows summary statistics for the score column.

What this step taught me:
Numeric columns can be explored using summary statistics such as mean, min, and max.

Full code:
```import pandas as pd

df = pd.read_csv("students.csv")

print("Dataset preview:")
print(df.head())

print("\nColumns:")
print(df.columns)

print("\nShape:")
print(df.shape)

print("\nMissing values in 'score':")
print(df["score"].isnull().sum())

print("\nScore statistics:")
print(df["score"].describe())```

## My Practice Result

From this practice, I found that:

- the dataset has 5 rows and 3 columns
- the columns are `name`, `age`, and `score`
- the `score` column has no missing values
- the average score is 86.8
- the minimum score is 76
- the maximum score is 95
