# NLP & Sequence Models

> Recurrent networks for text, plus a deep dive into LLM red-teaming. Three notebooks that cover how sequence models read, learn, and break.

This repo focuses on language. The first two notebooks build RNN and BiLSTM models from the ground up — useful both as working classifiers and as teaching material for how recurrent architectures actually process text. The third is a full red-teaming walkthrough on modern LLMs — adversarial prompting, jailbreak categories, and defensive evaluation.

---

## 📓 Notebooks in this repo

### 1. BiLSTM RNN — 94% Accuracy on Text Classification 📈
A bidirectional LSTM for sentiment / text classification, trained from scratch with a clear walkthrough of every piece — embeddings, sequence padding, the bidirectional layer, and why dropout matters in recurrent nets. Lands at 94% accuracy with a model small enough to train in a single Kaggle session.

📔 **[Open on Kaggle →](https://www.kaggle.com/code/samanfatima7/crushing-it-bilstm-rnn-delivers-94-accuracy)**

---

### 2. Decoding How RNNs Read Text 🤖🔍
Less a competition entry, more a *how does this thing actually work* notebook. Step through what happens inside an RNN cell as it reads a sentence — hidden states, the vanishing-gradient problem, why GRUs and LSTMs were invented. If you've ever wanted to *understand* RNNs instead of just import them, start here.

📔 **[Open on Kaggle →](https://www.kaggle.com/code/samanfatima7/decoding-how-rnns-read-text)**

---

### 3. A Complete Red-Teaming Walkthrough 💫🫣
A practical guide to red-teaming language models — prompt injection, jailbreak taxonomies, refusal evaluation, and how to build a structured test suite. Written for ML engineers who are starting to think about safety as a first-class concern rather than an afterthought.

📔 **[Open on Kaggle →](https://www.kaggle.com/code/samanfatima7/a-complete-red-teaming-walkthrough)**

---

## 🛠 Stack

Python · TensorFlow / Keras · PyTorch · NLTK · spaCy · transformers · OpenAI / Llama (red-teaming)

## 📂 How this repo is organized

Each notebook is standalone. To run locally:

```bash
git clone https://github.com/samanfatima7/nlp-and-sequence-models.git
cd nlp-and-sequence-models
pip install -r requirements.txt
jupyter notebook
```

The red-teaming notebook expects an LLM endpoint (OpenAI, Groq, or local Llama via Ollama) — set the relevant API key as an environment variable.

## 🧭 Why these three?

NLP is split into two eras — pre- and post-transformer. The RNN notebooks belong to the first era but the *intuition* they build (what is a sequence, how does context flow, where do gradients fail) is still load-bearing for understanding modern models. The red-teaming notebook is firmly in the second era — once your models work, the next problem is making sure they don't *misbehave*.

## 👋 About

Saman Fatima — Kaggle Legacy Grandmaster, data scientist from Pakistan. More work on [Kaggle](https://www.kaggle.com/samanfatima7) · [LinkedIn](https://www.linkedin.com/in/saman-fatima-datascience/) · [lablab.ai](https://lablab.ai/u/@safima__).

⭐ if any of these were useful — and if you're red-teaming production LLMs, I'd love to compare notes.
