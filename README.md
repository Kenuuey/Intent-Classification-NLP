# Understanding Customer — Intent Classification

This project introduces **Deep Learning for Natural Language Processing (NLP)** with a focus on **Intent Classification** — identifying what a user wants based on their text input.  
Example:  
> “Is it raining?” → intent: *ask about weather*


## 🧩 Overview

We explore how NLP models evolved from **rule-based chatbots** like ELIZA to modern **Transformer-based** architectures such as **BERT**.

This project offers **hands-on experience** with key deep learning architectures for text understanding:
- **Recurrent Neural Networks (RNN)**
- **Long Short-Term Memory (LSTM)** networks
- **Transformers**
- **BERT (Bidirectional Encoder Representations from Transformers)**

It also introduces essential NLP concepts such as **sequence modeling**, **context representation**, and **transfer learning**.


## 💬 Preamble

The journey of conversational AI began with **ELIZA**, a 1960s chatbot that simulated a therapist.  
ELIZA worked by identifying **keywords** and applying **transformation rules** to generate responses.

Today’s chatbots follow similar principles:
1. **Classify user intent** – What does the user want?  
2. **Generate or retrieve a relevant response.**

Example:  
> “What’s the temperature right now?” and “Is it raining?” → both map to the same intent: *ask about weather.*


## 🔍 Introduction

### Why Specialized Architectures for Text?

Unlike tabular data, text is **sequential** — word order and context matter.  
Deep learning provides several architectures that effectively model sequences:

- **RNN:** Processes sequences step by step but struggles with long-term dependencies.  
- **LSTM:** Introduces *memory gates* to retain and control contextual information.  
- **Transformer:** Uses an **attention mechanism** to process entire sequences in parallel, improving speed and context handling.  
- **BERT:** A **bidirectional Transformer** that learns deep contextual representations of language.

Training such models from scratch is computationally expensive, so we leverage **transfer learning** — fine-tuning pre-trained models on domain-specific data for powerful results.


## 📂 Project Structure
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