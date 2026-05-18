GitHub Title

Week 2 Part C — Train Set vs Test Set

⸻

File Name

notes/week2_partC_train_set_vs_test_set.md

⸻

GitHub Note Content

# Week 2 Part C — Train Set vs Test Set
## What I Learned
In this part, I learned the difference between a train set and a test set in machine learning.
Machine learning models do not simply memorize answers.
Instead, they try to learn patterns from data.
To properly evaluate a machine learning model, we usually split the dataset into:
- a train set
- a test set
---
# Train Set
A train set is the data used to train the model.
The model learns patterns from this data.
Example:
```text
study_hours → exam_score
2 → 60
4 → 78
6 → 92
```
The model tries to learn the relationship between:
- study hours
- exam scores
---
# Test Set
A test set is data that the model has never seen before.
The purpose of the test set is to check whether the model truly learned the pattern.
Example:
```text
5 → ?
```
The model predicts:
```text
84
```
Then we compare it with the actual answer:
```text
86
```
If the prediction is close to the real answer, the model is performing well.
---
# Why We Need a Test Set
If we use all data for training, the model may simply memorize the answers.
This is called:
# Overfitting
Overfitting means:
- the model performs well on training data
- but performs poorly on new data
A good machine learning model should be able to work on unseen data.
This is called:
# Generalization
---
# Real-Life Analogy
Train Set:
- like homework or practice questions
Test Set:
- like a real exam
A student who only memorizes practice questions may fail when the exam questions change.
Machine learning models behave similarly.
---
# Common Dataset Split
A common split is:
| Dataset Part | Percentage |
|---|---|
| Train Set | 80% |
| Test Set | 20% |
Other common splits:
- 70 / 30
- 75 / 25
---
# Example Workflow
Suppose we have 1000 rows of data.
```text
800 rows → Train Set
200 rows → Test Set
```
Workflow:
```text
1. Train the model using the train set
2. The model learns patterns
3. Test the model using the test set
4. Evaluate the prediction performance
```
---
# Important Concepts
| Concept | Meaning |
|---|---|
| Train Set | Data used for learning |
| Test Set | Data used for evaluation |
| Overfitting | Memorizing instead of learning |
| Generalization | Performing well on unseen data |
---
# Key Understanding
Machine learning is not about memorizing answers.
A good model should:
- learn patterns
- make predictions
- perform well on new unseen data
Train Set helps the model learn.
Test Set checks whether the model truly understands the pattern.
