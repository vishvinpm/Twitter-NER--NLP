# Twitter NER Case Study 🚀

This project is a deep learning-based **Named Entity Recognition (NER)** system built to identify entities (like names, locations, brands, etc.) in **Twitter text**, which is often informal, noisy, and context-rich.

---

## 📌 Problem Statement

Named Entity Recognition on Twitter data poses unique challenges due to:
- Short and noisy text
- Misspellings and abbreviations
- Unstructured grammar

Our goal: **Build a robust NER model** that can accurately detect entities in tweets using deep learning and custom embeddings.

---

## 🧠 Approach

- **Data Preprocessing**: Tokenization, padding, and handling unknown tokens.
- **Embedding**: Trained custom Word2Vec embeddings on Twitter corpus.
- **Model Architecture**:
  - BiLSTM layers
  - TimeDistributed Dense
  - CRF (Conditional Random Field) for sequence labeling
- **Loss Function**: `Sigmoid Focal Cross-Entropy` for class imbalance.
- **Evaluation**: Accuracy, Precision, Recall, F1-score using `seqeval`.
