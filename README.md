# Probabilistic ML Thinking (Naive Bayes) — FAANG-Level Hands-On

**Goal:** Build probabilistic intuition for generative modeling and implement Naive Bayes from scratch.

**Outcome:** Students can explain generative vs discriminative modeling, conditional independence assumptions, and implement Naive Bayes for text classification (log-space, Laplace smoothing).

---

# How to Start

1. **Fork** this repository.  
2. Open `nb_student_lab.ipynb` in **Google Colab**.  
3. Complete all **TODO** sections.  
4. **Restart runtime → Run All** cells.  
5. Push changes and submit a **Pull Request**.  

⚠️ **Do NOT edit notebooks directly on GitHub.**

---

## Lab Rules (FAANG Style)

- ✅ Work in log-space (avoid underflow)
- ✅ Use Laplace smoothing
- ✅ Explicitly state independence assumptions
- ✅ Do slice-based error analysis (which words/classes fail?)

---

# Out of Scope

- scikit-learn Naive Bayes (we implement ourselves)
- Deep NLP

---

# Notebook Rules

- Do **NOT** rename the notebook  
- Do **NOT** delete TODOs  
- Do **NOT** hardcode outputs  
- Notebook must run **top-to-bottom**  

---

# Dataset

- Small synthetic text dataset (always works)
- Optional: plug in a Kaggle/UCI text dataset later (Week 4+)

## Why?

- Mirrors interview-style toy setups
- Forces focus on probabilistic reasoning

---

## Section 1 — Generative vs Discriminative

### Task 1.1: Explain modeling choices

**Checkpoint Questions:**

- What does Naive Bayes model that logistic regression does not?
- When can a “wrong” generative assumption still work well?

---

## Section 2 — Multinomial Naive Bayes

### Task 2.1: Build vocabulary + count vectors

**FAANG Gotcha:**

- Tokenization edge cases (case, punctuation)

---

### Task 2.2: Train NB with Laplace smoothing

**Checkpoint Questions:**

- Why smoothing is required?
- What happens with unseen words?

---

### Task 2.3: Predict in log-space

**Interview Angle:**

- Why log converts products into sums?

---

## Section 3 — Error Analysis

### Task 3.1: Inspect most influential tokens

- Show top tokens per class using learned log probabilities

---

## Submission Expectations

- Completed notebook
- Short written answers to checkpoint questions
- Show accuracy + confusion matrix on the toy dataset

---

## FAANG Interview Evaluation Rubric

| Skill                        | Evaluated |
|-----------------------------|-----------|
| Probabilistic reasoning     | ✅        |
| Numerical stability (logs)  | ✅        |
| Smoothing intuition         | ✅        |
| Error analysis              | ✅        |
| Code clarity                | ✅        |

---

## Stretch Problems (Optional)

- Bernoulli NB (presence/absence)
- Handle bigrams
- Add class imbalance priors
