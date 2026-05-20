# Week 2 Part F — Basic Evaluation

## What is Evaluation?

Evaluation means checking how good the model’s predictions are.

It helps us understand:

- whether the model predicts correctly
- whether the model performs well on new data

---

# Prediction Error

Prediction Error means:

difference between predicted value and actual value.

## Formula

$begin:math:display$
\\text\{Error\} \= \\text\{Predicted Value\} \- \\text\{Actual Value\}
$end:math:display$

### Example

- Actual score: 90
- Predicted score: 85

Error:

```text
85 - 90 = -5
```

The model missed by 5 points.

---

# Accuracy

Accuracy is commonly used for classification problems.

It measures:

how many predictions are correct.

## Formula

$begin:math:display$
\\text\{Accuracy\} \= \\frac\{\\text\{Correct Predictions\}\}\{\\text\{Total Predictions\}\}
$end:math:display$

### Example

- 10 predictions
- 8 correct
- 2 wrong

Accuracy:

```text
8 / 10 = 0.8 = 80%
```

---

# Mean Squared Error (MSE)

For regression problems, a common metric is:

Mean Squared Error (MSE)

MSE:

1. calculates error
2. squares the error
3. averages the result

## Formula

$begin:math:display$
MSE \= \\frac\{1\}\{n\}\\sum \(y\_\{true\} \- y\_\{pred\}\)\^2
$end:math:display$

---

# Important Understanding

Smaller MSE = Better Model

---

# Why Square the Error?

Because:

- positive and negative errors will not cancel each other
- large errors are punished more heavily

| Error | Squared |
|---|---|
| 2 | 4 |
| 10 | 100 |

---

# sklearn Evaluation Example

```python
from sklearn.metrics import mean_squared_error

mse = mean_squared_error(y_true, y_pred)
```

This calculates model prediction error.

---

# Train Accuracy vs Test Accuracy

## High Train Accuracy

The model performs well on training data.

## High Test Accuracy

The model also performs well on new unseen data.

This is more important.

---

# Overfitting

Overfitting happens when the model memorizes training data instead of learning patterns.

### Example

- Train accuracy: 99%
- Test accuracy: 52%

This means:

the model memorized answers but cannot generalize well.

---

# Key Summary

| Concept | Meaning |
|---|---|
| Evaluation | Checking model performance |
| Error | Difference between prediction and real value |
| Accuracy | Percentage of correct predictions |
| MSE | Average squared error |
| Overfitting | Memorizing instead of learning |

---

# My Understanding

Machine learning models must be evaluated to measure prediction quality.

- Accuracy is commonly used for classification problems.
- MSE is commonly used for regression problems.
- Good models should perform well on unseen test data.

A model that only memorizes training data may suffer from overfitting.

---

# Quick Check

1. What does evaluation mean in ML?
2. What is prediction error?
3. Which metric is common for classification?
4. Which metric is common for regression?
5. What is overfitting?

---

