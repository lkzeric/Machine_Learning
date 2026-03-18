# Machine Learning (Final Project for ML)

**Authors:**  
Kuo-Jui Lan, Jaehyung Choi  

**Deadline:**  
March 20, 2026

---

# 1. Project Overview

This project implements a **sentiment analysis model** for movie reviews using the **IMDB dataset**.  
The model is based on **DistilBERT as a text encoder** combined with a **multi-layer perceptron (MLP)** classifier.

A **two-stage training strategy** is applied to improve training stability and leverage pretrained language representations.

The system takes **raw text reviews** as input and predicts the sentiment label (**positive or negative**).

---

# 2. Goal

The goal of this project is to explore the effectiveness of **transformer-based models** for sentiment classification.

Specifically, we investigate how **DistilBERT representations combined with a simple MLP classifier** perform on the **IMDB movie review dataset**.

We also evaluate different training strategies, including a **two-stage training procedure**, and analyze their impact on model performance.

---

# 3. Dataset

### IMDB Dataset of 50K Movie Reviews

Dataset link:

https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

---

# 4. Setup Instructions

- Python 3.14.3

---

# 5. Dependencies

- Python >= 3.9
- PyTorch
- Transformers (HuggingFace)
- scikit-learn
- pandas
- numpy
- tqdm
- scipy

---

# 6. How to Train / Evaluate the Model

We provide **three notebooks** in our repository.  
They can be executed with **Jupyter Notebook**.

### Baseline Models

- `linear_regression.ipynb`
- `SVD_Clustering.ipynb`

### Advanced Model

- `DistilBERT_MLP.ipynb`

---

# 7. Expected Outputs

## Baseline Models

### Evaluation Metrics

Both models report:

- Accuracy
- Precision
- Recall
- F1 Score

Additional outputs:

- **Linear Regression**
  - Loss
  - Top 10 negative / positive words

- **Clustering**
  - K-means convergence

### Interaction Interface

- The user can input a sentence, and the model will classify whether the sentiment is **positive or negative** until the user types `quit`.

---

## Advanced Model (DistilBERT + MLP)

### Evaluation Metrics

- Validation accuracy
- Confusion matrix
- ROC curve
- Training curve

### Interaction Interface

- The user can input a sentence, and the model will classify whether the sentiment is **positive or negative**.