# ✍️ Handwritten Mathematical Equation Recognition

A deep learning pipeline to recognize and convert handwritten mathematical expressions into LaTeX markup using CNNs, Transformers, and hybrid architectures.

---

## 🧠 Project Overview

This project explores the problem of recognizing handwritten mathematical expressions and converting them to their equivalent LaTeX representations. We implement and compare three different neural network models:

1. **CNN + LSTM** – A baseline model with sequential decoding
2. **ResNet + Transformer Decoder** – Utilizes a ResNet18 encoder with Transformer decoding
3. **ResNet + Positional Transformer (Posformer)** – Combines a ResNet encoder with a positional-aware transformer decoder

---

## 📊 Dataset

We used the [**Handwritten Mathematical Expressions Dataset**](https://www.kaggle.com/datasets/rtatman/handwritten-mathematical-expressions) from Kaggle, which includes:

- ~11,000 images of handwritten equations
- LaTeX annotations
- A wide range of mathematical symbols including `\frac`, `\int`, `\sum`, and trigonometric functions

📦 **Setup**:  
Download and extract the dataset into the `data/` folder before running the code.

---

## 🏗️ Model Architectures

| Model                         | Description                                                 |
|------------------------------|-------------------------------------------------------------|
| CNN + LSTM                   | Baseline model with feature extraction + sequential decoding |
| ResNet + Transformer         | Deep ResNet18 encoder + Transformer decoder                 |
| ResNet + Positional Transformer | Incorporates 2D positional encoding in decoder              |

---

## 📈 Evaluation Metrics

| Metric                  | CNN+LSTM | ResNet+Transformer | ResNet+Posformer |
|-------------------------|----------|--------------------|------------------|
| Token-Level Accuracy    | 69.18%   | 74.12%             | **81.07%**       |
| Exact Match Accuracy    | 30.73%   | 31.37%             | **35.07%**       |
| Character Error Rate    | 0.4314   | 0.4131             | **0.2372**       |
| BLEU Score              | 0.3312   | 0.4223             | **0.5944**       |

---

✍️ Authors

1. Du, Miranda
2. Liu, Tianze
3. Mathi, Vandana
4. Polapragada, Saivenkata Nagavyjayanthi

---

📚 References

1. Dataset: Rachael Tatman, Kaggle
2. Vaswani et al. (2017), “Attention is All You Need”
3. Kingma & Ba (2014), “Adam: A Method for Stochastic Optimization”
