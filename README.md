# Understanding Customer — Intent Classification

This project introduces **Deep Learning for Natural Language Processing (NLP)** with a focus on **Intent Classification** — identifying what a user wants based on their text input.  
Example:  
> “Is it raining?” → intent: *ask about weather*


## Overview

We explore how NLP models evolved from **rule-based chatbots** like ELIZA to modern **Transformer-based** architectures such as **BERT**.

This project provides a **hands-on experience** with key deep learning models for text understanding::
- **Recurrent Neural Networks (RNN)**
- **Long Short-Term Memory (LSTM)**
- **Transformers**
- **BERT (Bidirectional Encoder Representations from Transformers)**

and introduces key NLP concepts such as **sequence modeling**, **context understanding**, and **transfer learning**.

## Preamble

The journey of conversational AI began with **ELIZA**, a 1960s chatbot that simulated a therapist.  
ELIZA worked by identifying **keywords** and applying **transformation rules** to generate responses.

Today’s chatbots follow similar principles:
1. **Classify user intent** – What does the user want?  
2. **Generate or retrieve a relevant response.**

Example:  
> “What’s the temperature right now?” and “Is it raining?” → both map to the same intent: *ask about weather.*


## Introduction

### Why Specialized Architectures for Text?

Unlike tabular data, text is **sequential** — order matters.  
Deep learning offers several architectures for handling text:

- **RNN:** Processes sequences but forgets long-term context.  
- **LSTM:** Adds “memory gates” to retain context.  
- **Transformer:** Uses an **attention mechanism** to process sequences in parallel, understanding context globally.  
- **BERT:** A bidirectional Transformer pre-trained for deep contextual understanding.

Training these models from scratch is expensive, so we use **transfer learning** — fine-tuning pre-trained models on our data for powerful results.


## 📊 Project Structure
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