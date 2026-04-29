# 🧠 Natural Language Processing (NLP) — Learning Series

This repository documents my structured journey of learning **Natural Language Processing (NLP)** from scratch, focusing on building strong intuition along with practical implementation in Python.

---

## 🚀 What This Repo Covers

* 🔤 Text Preprocessing Pipeline
* 📊 Bag of Words & TF-IDF
* 🧠 Word Embeddings (Word2Vec)

---

## 🎯 Goal

The goal of this repository is not just to implement models, but to:

* Understand the **intuition behind each concept**
* Learn **how and why** each technique is used
* Build a **strong foundation in NLP and Deep Learning**

---

Each folder contains:

* 📘 Explanation (notes)
* 💻 Code implementation
* 🧠 Key insights

---

## 🛠️ Tech Stack

* Python
* NLTK
* scikit-learn

---

## 📌 Key Learning Approach

* Start with **basic intuition**
* Move to **mathematical understanding**
* Then implement using code
* Finally, connect concepts to real-world applications

---

## 🔥 Why This Repo?

Many resources jump directly into complex theory.
This repo focuses on:
👉 Learning concepts in the simplest possible way
👉 Building clarity step-by-step
👉 Making NLP beginner-friendly

---

## 📅 Progress

* ✅ Day 1: Text Preprocessing
* ✅ Day 2: TF-IDF & Word Embeddings

---
## 📍 Day 3: Sentiment Classifier

Built a basic sentiment classification pipeline using:
- TF-IDF + Logistic Regression
- Word2Vec (with sentence vector averaging)

 ## 📍 Day 4: RNN & Embeddings (Step 1)

Today marks the transition from traditional NLP to **Deep Learning for text**.

---

## 🧠 What Problem Are We Solving?

Earlier approaches (TF-IDF, Word2Vec averaging) had a key limitation:

👉 They ignore **word order (sequence)**

Example:

* "I love AI"
* "AI love I"

Both look similar to traditional models ❌
But meaning is clearly different.

---

## 🔥 Introduction to RNN (Recurrent Neural Network)

RNNs are designed to process **sequential data**.

👉 Instead of reading the whole sentence at once,
they process it **word by word** while maintaining a **memory (hidden state)**.

---

## 🔄 RNN Flow

```id="k6r9dr"
Word₁ → Word₂ → Word₃ → ... → Prediction
        ↓
     Memory (Hidden State)
```

---

## 🧠 Key Insight

👉 Meaning in language depends on **order and context**, not just words.

---

## 🔢 Step 1: Text → Numerical Sequences

Before feeding text into RNN:

* Build a vocabulary → word → index
* Convert sentences → sequence of integers

Example:

```id="u9d5nq"
"I love AI" → [1, 2, 3]
```

---

## ⚠️ Limitation of Basic Encoding

👉 These numbers are just IDs
👉 They **do NOT capture meaning**

Example:

* "love" = 2
* "hate" = 5

No relationship between them ❌

---

## 💡 Introduction to Embedding Layer

To solve this, we use an **Embedding Layer**.

👉 Instead of:

```id="qjzqmb"
word → number
```

👉 We learn:

```id="zdc9f4"
word → vector (meaningful representation)
```

---

## 🧠 Why Embeddings Matter

* Words with similar meaning → similar vectors
* Model learns relationships automatically
* Much better representation than raw indices

---

## 🔥 Updated Pipeline

```id="n0d4xz"
Text → Tokenization → Encoding → Embedding → RNN → Prediction
```

---

## 🎯 Key Learnings

* RNNs process sequences (order matters)
* Encoding converts text into numerical form
* Embeddings transform IDs into meaningful vectors
* Representation plays a crucial role in deep learning

---

## 🚀 Next Step

* Understanding how RNN processes sequences internally
* Hidden states and how memory evolves
* Limitations of RNN → leading to LSTM

---


### Key Learnings:
- ML models require fixed-size input vectors
- TF-IDF provides sentence-level features directly
- Word2Vec provides word-level embeddings → needs aggregation
- Representation of text plays a crucial role in model performance

### Pipeline:
Text → Preprocessing → Vectorization → Model → Prediction

## 🤝 Connect

I’m also sharing daily insights from this journey on LinkedIn.
Feel free to connect and follow along!

---

⭐ If you find this helpful, consider starring the repo!

