# Week 2 Part 1 — Basic Machine Learning Terms

## What I Learned

In this part, I learned five basic machine learning terms:

- dataset
- sample
- feature
- label
- target

These terms are important because they help me understand how machine learning problems are structured.

---

## Dataset

A dataset is the full collection of data used in a machine learning project.

For example, if we have a table of student information, the whole table is the dataset.

Example:

| student | study_hours | sleep_hours | attendance | final_score |
|---|---:|---:|---:|---:|
| A | 2 | 6 | 80 | 65 |
| B | 5 | 8 | 95 | 88 |
| C | 1 | 5 | 70 | 55 |

In this example, the entire table is the dataset.

---

## Sample

A sample is one row in the dataset.

Each row usually represents one data point.

For example:

| student | study_hours | sleep_hours | attendance | final_score |
|---|---:|---:|---:|---:|
| B | 5 | 8 | 95 | 88 |

This row is one sample because it describes one student.

---

## Feature

A feature is an input variable used by the machine learning model to make predictions.

In the student example, the features are:

- study_hours
- sleep_hours
- attendance

These are the pieces of information the model uses to learn patterns.

---

## Label / Target

A label, also called a target, is the value we want the model to predict.

In the student example, the target is:

- final_score

The model uses the features to predict the target.

So the machine learning problem is:

```text
study_hours + sleep_hours + attendance → final_score
