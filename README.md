# 🎬 Movie Review Sentiment Classification

This project uses a deep learning model (Bidirectional LSTM with GloVe embeddings) to classify IMDb movie reviews as **Positive** or **Negative**.

---

## 📌 Overview

This sentiment classification task uses a dataset of IMDb movie reviews with binary sentiment labels (positive or negative). The goal is to build a robust NLP pipeline that performs effective sentiment classification using deep learning techniques.

---

## 📂 Dataset

- Total labeled reviews: **50,000**
- **25,000** training (balanced)
- **25,000** testing (balanced)
- **50,000 unlabeled** reviews for unsupervised learning (not used in this project)

**Label definition:**
- **Positive**: Rating ≥ 7 out of 10  
- **Negative**: Rating ≤ 4 out of 10  
- Neutral reviews are excluded.

📝 Notes:
- No more than 30 reviews per movie (to avoid bias).
- Training and testing sets contain **disjoint movie sets**.
- Dataset is sourced from [IMDb](https://ai.stanford.edu/~amaas/data/sentiment/).

---

## 🧠 Model Architecture

- **Embedding Layer**: GloVe (50d), frozen
- **Bidirectional LSTM**: 128 units
- **Dense Layer**: 64 neurons, ReLU
- **Dropout**: 0.5 and 0.3
- **Output**: Sigmoid (binary classification)

---

## 🏁 Performance

| Metric     | Value    |
|------------|----------|
| Accuracy   | 84.46%   |
| Precision  | 81.57%   |
| Recall     | 89.19%   |
| F1-score   | 85.21%   |

🔍 Confusion matrix and ROC curve are saved as images in the repo.




## 🚀 How to Use




