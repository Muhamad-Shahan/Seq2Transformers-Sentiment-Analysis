# 📜 From Sequences to Transformers: LSTM and BERT Powering Next-Gen Sentiment Analysis

[![Journal](https://img.shields.io/badge/Journal-IJISCT-blue.svg)](https://journals.cfrit.com/index.php/ijisct/article/view/139)
[![Paper](https://img.shields.io/badge/Paper-PDF-red.svg)](docs/Published_Paper_IJISCT.pdf)
[![Model](https://img.shields.io/badge/Model-BERT%20Fine--Tuned-green.svg)]()
[![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)]()

## 📌 Abstract
This repository contains the official source code and experimental logs for the research paper **"From Sequences to Transformers: LSTM and BERT Powering Next-Gen Sentiment Analysis"**, published in the *International Journal of Information Systems and Computer Technologies (IJISCT)*.

Customer feedback is a potent source of insight, but traditional recurrent networks often fail to capture semantic ambiguity and sarcasm. This study presents a rigorous comparative analysis of **Long Short-Term Memory (LSTM)** networks versus **Bidirectional Encoder Representations from Transformers (BERT)**.

Using a dataset of **50,000 Amazon Food Reviews**, we demonstrate that the Transformer-based approach significantly outperforms recurrent architectures in handling long-range dependencies and contextual nuance.

> **[📄 Read the Full Paper](https://journals.cfrit.com/index.php/ijisct/article/view/139)**

## 📊 Key Results
Our experiments were conducted under identical protocols to ensure a fair comparison. BERT achieved Superior performance across all metrics.

| Metric | LSTM (Baseline) | BERT (Proposed) | Improvement |
| :--- | :--- | :--- | :--- |
| **Accuracy** | 84.2% | **88.2%** | +4.0% |
| **F1-Score** | 0.843 | **0.883** | +0.04 |
| **ROC-AUC** | 0.901 | **0.942** | +0.04 |

## 🧠 Methodology

### 1. Baseline: LSTM
* **Embedding:** Learned 128-dimensional word embeddings.
* **Architecture:** Single-layer LSTM (64 units) with `tanh` activation.
* **Regularization:** Dropout (0.5) to prevent overfitting.
* **Optimizer:** Adam.

### 2. Proposed: BERT (Fine-Tuned)
* **Base Model:** `bert-base-uncased` (110M parameters).
* **Tokenization:** WordPiece tokenization with dynamic padding.
* **Fine-Tuning:** Trained for 3 epochs with a learning rate of 2e-5.
* **Contextualization:** Utilizes self-attention mechanisms to understand bidirectional context.

## 📚 Citation
If you utilize this code or our findings in your research, please cite the paper as follows:

**BibTeX:**
```bibtex
@article{ibad2024sequences,
  title={From Sequences to Transformers: LSTM and BERT Powering Next-Gen Sentiment Analysis},
  author={Khan, Mohammad Arbi and Khalid, Afsheen and Ibad, Muhammad Shahan and Khan, Dilawar and Malik, Fazal},
  journal={International Journal of Information Systems and Computer Technologies},
  volume={5},
  number={1},
  year={2024},
  publisher={CFRIT},
  url={[https://journals.cfrit.com/index.php/ijisct/article/view/139](https://journals.cfrit.com/index.php/ijisct/article/view/139)},
  doi={10.58325/ijisct.004.02.00139}
}
```
## 👥 Authors

This research was a collaborative effort between the following institutions:

* **Mohammad Arbi Khan**¹
    * *Institute of Management Sciences (IMSciences), Peshawar*
* **Afsheen Khalid**²
    * *University of Engineering and Technology (UET), Peshawar*
* **Muhammad Shahan Ibad**¹ (Corresponding Author) 📧
    * *Institute of Management Sciences (IMSciences), Peshawar*
* **Dilawar Khan**¹
    * *Institute of Management Sciences (IMSciences), Peshawar*
* **Fazal Malik**³
    * *Iqra National University, Peshawar*

---
*¹ School of Computer Science and Information Technology, IMSciences*
*² Department of Computer Science, UET Peshawar*
*³ Department of Computer Science, Iqra National University*
