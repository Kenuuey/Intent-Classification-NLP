# 🧠 Understanding Customer — Intent Classification

This project introduces **Deep Learning for Natural Language Processing (NLP)** with a focus on **Intent Classification** — identifying what a user wants based on their text input.  
Example:  
> “Is it raining?” → intent: *ask about weather*

---

## 🚀 Overview

You’ll explore how NLP models evolved from **rule-based chatbots** like ELIZA to modern **Transformer-based** architectures such as **BERT**.

This project provides a **hands-on experience** with:
- **Recurrent Neural Networks (RNN)**
- **Long Short-Term Memory (LSTM)**
- **Transformers**
- **BERT (Bidirectional Encoder Representations from Transformers)**

and introduces key NLP concepts such a

---

## Chapter I – Preamble

The journey of conversational AI began with **ELIZA**, a 1960s chatbot that simulated a therapist.  
ELIZA worked by identifying **keywords** and applying **transformation rules** to generate responses.

Today’s chatbots follow similar principles:
1. **Classify user intent** – What does the user want?  
2. **Generate or retrieve a relevant response.**

Example:  
> “What’s the temperature right now?” and “Is it raining?” → both map to the same intent: *ask about weather.*

---

## Chapter II – Introduction

### 🧠 Why Specialized Architectures for Text?

Unlike tabular data, text is **sequential** — order matters.  
Deep learning offers several architectures for handling text:

- **RNN:** Processes sequences but forgets long-term context.  
- **LSTM:** Adds “memory gates” to retain context.  
- **Transformer:** Uses an **attention mechanism** to process sequences in parallel, understanding context globally.  
- **BERT:** A bidirectional Transformer pre-trained for deep contextual understanding.

Training these models from scratch is expensive, so we use **transfer learning** — fine-tuning pre-trained models on our data for powerful results.

---

## Chapter III – Rules of Project

- Use **Python 3**.  
- You can organize your files freely, but keep the structure clean.  
- You may use **Google Colab** for training (GPU recommended).  
- Place datasets inside the `data/` folder.  
- Keep a **research journal** to track model changes, hyperparameters, and metrics.

---

## Chapter IV – Instructions

1. Use any framework: **PyTorch**, **TensorFlow**, or **Keras**.  
2. Save your trained model in **Pickle (.pkl)** format.  
3. The notebook(s) must include:
   - Data preprocessing  
   - Model training (RNN, LSTM, BERT)  
   - Evaluation (accuracy ≥ 0.8 on test set)  
4. Predictions should be saved to `intents.csv`.  

> **Fallback Intent:**  
> Include handling for unseen queries (e.g., “I couldn’t understand you.”).  
> This improves chatbot robustness and evaluation score.

---

## 📊 Example Folder Structure
```
├── data/
│ ├── intents_train.csv
│ ├── intents_test.csv
├── notebooks/
│ ├── rnn_model.ipynb
│ ├── lstm_model.ipynb
│ ├── bert_model.ipynb
├── models/
│ ├── rnn.pkl
│ ├── lstm.pkl
│ ├── bert.pkl
├── intents.csv
├── research_journal.md
└── README.md
```