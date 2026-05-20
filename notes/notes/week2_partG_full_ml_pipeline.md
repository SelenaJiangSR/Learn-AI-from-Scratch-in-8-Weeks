# Week 2 Part G — Understanding the Full ML Pipeline

## What is a Machine Learning Pipeline?

A machine learning pipeline is the complete workflow of a machine learning project.

It describes the full process:

from data collection to prediction and evaluation.

---

# The Full ML Pipeline

```text
Collect Data
     ↓
Prepare Data
     ↓
Split Data
     ↓
Choose Model
     ↓
Train Model
     ↓
Make Predictions
     ↓
Evaluate Model
```

This is one of the most important structures in machine learning.

---

# Step 1 — Collect Data

The first step in ML is collecting data.

### Examples

## Netflix

Collects:

- watch history
- liked movies
- viewing time

## House Price Prediction

Collects:

- house size
- location
- number of bedrooms
- house price

## Spam Detection

Collects:

- email text
- spam labels

---

# Important Understanding

Better Data > Better Model

In many real-world projects, data quality is more important than the model itself.

---

# Step 2 — Prepare Data

Real-world data is usually messy.

So we need:

Data Cleaning

### Common Problems

| Problem | Example |
|---|---|
| Missing values | empty cells |
| Wrong formats | text instead of numbers |
| Duplicate data | repeated rows |
| Noise | incorrect values |

---

# Step 3 — Split Data

Split the dataset into:

- training set
- testing set

### Why?

Because we want to test the model on new unseen data.

Not just memorized training data.

---

# Step 4 — Choose a Model

Different problems require different models.

## Regression Problems

Possible model:

- Linear Regression

## Classification Problems

Possible models:

- Logistic Regression
- Decision Tree

---

# Important Idea

Different Problems → Different Models

---

# Step 5 — Train the Model

```python
model.fit(X_train, y_train)
```

The model starts learning patterns from data.

### Example

More study hours → higher scores

---

# Step 6 — Make Predictions

```python
model.predict([[6]])
```

Example prediction:

6 study hours → 100 score

---

# Step 7 — Evaluate the Model

After prediction, we evaluate model performance.

## Classification

Common metric:

- Accuracy

## Regression

Common metric:

- Mean Squared Error (MSE)

---

# Goal of Evaluation

A good model should perform well on unseen test data.

---

# Real-World Example — YouTube Recommendation System

## Step 1 — Collect Data

Collect:

- watch history
- likes
- viewing time

## Step 2 — Prepare Data

Clean incorrect or messy data.

## Step 3 — Split Data

Create train/test datasets.

## Step 4 — Choose Model

Use recommendation algorithms.

## Step 5 — Train

Learn user behavior patterns.

## Step 6 — Predict

Predict videos users may like.

## Step 7 — Evaluate

Check whether users actually click the recommendations.

---

# The Big Picture

Machine learning is essentially:

```text
data → learning → prediction
```

A more complete version:

```text
data
 ↓
clean
 ↓
train
 ↓
predict
 ↓
evaluate
 ↓
improve
```

---

# Important Understanding

In real-world ML projects, the hardest part is often not the model.

It is the data.

Real-world data is usually:

- messy
- incomplete
- noisy

This is why Data Science is very important.

---

# What I Have Learned So Far

| Concept | Meaning |
|---|---|
| Dataset | Data collection |
| Feature | Input variable |
| Label / Target | Prediction target |
| Regression | Predict numbers |
| Classification | Predict categories |
| Train/Test Split | Data splitting |
| Model | Learning system |
| fit() | Training |
| predict() | Prediction |
| Evaluation | Model checking |
| Pipeline | Full ML workflow |

---

# My Understanding

A machine learning project follows a complete pipeline:

1. collect data
2. prepare data
3. split data
4. choose model
5. train model
6. make predictions
7. evaluate performance

Machine learning is fundamentally about learning patterns from data and using those patterns to make predictions.

---

# Huge Milestone

I have now completed the foundations of machine learning.

These concepts are the basis for future topics such as:

- Deep Learning
- AI Agents
- LLMs
- Computer Vision
- Recommendation Systems

---

