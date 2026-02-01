# Handling Imbalanced Datasets with Generative AI  
### Fraud Detection Case Study

Practical data science case developed after completing the **AI for Data** course at Rocketseat, focused on addressing **extreme class imbalance** in fraud detection using **Generative AI** for data augmentation.

---

## 📌 Problem Context

We are a data team at a fictional **fintech**, tasked with building a model to detect **fraudulent transactions**.

The main challenge:
- The dataset is **extremely imbalanced**
- More than **99% of transactions are legitimate**
- Fraud cases represent less than **1%** of the data

This imbalance makes it difficult for traditional machine learning models to correctly learn and identify fraudulent patterns.

---

## 🎯 Objective

- Demonstrate how a baseline ML model performs poorly on highly imbalanced data
- Use **Generative AI** to create **synthetic fraud samples**
- Retrain the model with the augmented dataset
- Validate and compare performance improvements

---

## 🧠 Strategy & Approach

### 1️⃣ Baseline Model
- Train a traditional ML model using the original dataset
- Evaluate its performance on fraud detection
- Observe low recall and poor fraud identification despite high overall accuracy

### 2️⃣ Synthetic Data Generation with GenAI
- Use **Gemini (Generative AI)** to generate realistic synthetic fraud transactions
- Ensure generated samples follow the same schema and constraints as the original dataset
- Increase the representation of the minority (fraud) class

### 3️⃣ Model Retraining
- Combine real and synthetic fraud samples
- Retrain the model on the augmented dataset
- Re-evaluate performance using appropriate metrics

---

## 📊 Evaluation Metrics

Given the imbalanced nature of the problem, the focus was placed on:
- Recall
- Precision
- F1-score
- Confusion Matrix

Accuracy alone was intentionally avoided as a primary metric.

---

## 🧪 Results & Findings

- The baseline model struggled to identify fraudulent transactions
- After data augmentation:
  - Recall for fraud detection improved significantly
  - The model demonstrated better sensitivity to minority class patterns
- The experiment highlights how **data quality and balance** can be more impactful than model complexity

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **Scikit-learn**
- **Machine Learning**
- **Generative AI (Gemini)**
- **Synthetic Data Generation**
- **Model Evaluation Metrics**

---

## ⚠️ Limitations & Considerations

- Synthetic data quality directly impacts model performance
- Generated samples may introduce bias if not properly constrained
- This approach complements, but does not replace, real-world fraud data
- Further validation would be required for production use

---

## 🤖 Use of AI Tools

Generative AI was intentionally used as a **data augmentation strategy**, not as a replacement for modeling decisions.

All generated samples were reviewed for consistency, schema validity, and logical coherence before being incorporated into the training dataset.

AI-assisted tools were also used during development to support experimentation and learning.

---

## 📂 Project Context

- Educational / experimental case study
- Developed as part of Rocketseat’s **AI for Data** program
- Focused on applied problem-solving rather than production deployment

---

## 🔎 Why this project matters

This project demonstrates:
- Understanding of real-world data imbalance challenges
- Proper evaluation of ML models beyond accuracy
- Practical application of Generative AI in data science
- Critical thinking about data quality, limitations, and validation
