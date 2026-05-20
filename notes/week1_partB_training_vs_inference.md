# ⚙️ Week 1 Part B — Training vs Inference

---

# 🏋️ Training

### 🧠 Explanation
Training is the process of teaching a model to learn patterns from data.

During training, the model sees a large amount of data and updates its parameters to improve performance.

### 💡 My Understanding
Training is when the model is learning from examples.

It gradually improves by adjusting itself again and again based on mistakes.

### 🚀 Example
If we train a model using thousands of cat and dog images:

- the model learns what cats look like
- the model learns what dogs look like
- the model improves over time

---

# ⚡ Inference

### 🧠 Explanation
Inference is the process of using a trained model to make predictions or generate outputs for new inputs.

### 💡 My Understanding
Inference is when the model uses what it already learned.

It is no longer studying — it is applying knowledge.

### 🚀 Example
After training:

- you upload a new image
- the model predicts:
  "This is a cat."

That prediction step is inference.

---

# 🔍 Key Difference

| Training | Inference |
|---|---|
| Learning | Using |
| Updates parameters | Uses fixed parameters |
| Expensive | Faster |
| Needs huge datasets | Uses new input data |
| Happens before deployment | Happens during real usage |

---

# 🤖 Why Normal ChatGPT Use is Inference

When ChatGPT answers questions, it uses already trained parameters to generate responses.

It is not retraining itself every time you send a message.

### 📌 Example

When you type:

> "Explain machine learning."

ChatGPT is:

- using learned knowledge
- generating predictions for the next word
- producing a response

This is inference.

---

# 💸 Why Training is More Expensive

Training requires:

- 📚 Large datasets
- 🔄 Repeated parameter updates
- 🖥️ Massive computation
- ⏳ Long running time
- ⚡ Powerful hardware such as GPUs

Large AI models may train for:

- weeks
- months
- sometimes even longer

using thousands of GPUs.

---

# 🌌 Big Picture

```text
Training
   ↓
Model learns patterns
   ↓
Model becomes trained
   ↓
Inference
   ↓
Model uses learned knowledge
```

---

# 🧭 Key Takeaways

- Training = learning from data
- Inference = using learned knowledge
- Training is much more computationally expensive
- Most normal AI product usage is inference
- ChatGPT conversations are inference, not training

---

# ✨ My Reflection

Before learning this, I thought AI systems were "learning live" during every conversation.

Now I understand that:

most AI systems are already trained beforehand.

When we use tools like ChatGPT, we are mainly interacting with the inference stage of AI.
