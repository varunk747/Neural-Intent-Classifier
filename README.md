# Neural Intent Classifier

![Status](https://img.shields.io/badge/Status-Legacy%20Archive-lightgrey) ![Python](https://img.shields.io/badge/Python-3.6%2B-blue) ![TensorFlow](https://img.shields.io/badge/TensorFlow-1.x%20Compat-orange)

### **Project Overview**
This repository contains a custom implementation of a **Deep Neural Network (DNN)** for Natural Language Understanding (NLU) and intent classification. 

Unlike modern Large Language Models (LLMs) that rely on heavy pre-trained transformers, this project demonstrates how to build a performant chatbot "brain" from scratch using:
* **Bag of Words (BoW)** for vectorization.
* **Feed-Forward Neural Networks** for classification.
* **Stemming & Tokenization** via NLTK.

### **Repository Structure**
* `Neural_Intent_Classifier.ipynb` - The core logic for data preprocessing, model training, and inference loop.
* `intents.json` - The dataset containing patterns and responses for training.
* `requirements.txt` - Dependencies required to reproduce the environment.

### **Technical Architecture**
The model is built using `TFLearn` (a high-level API for TensorFlow) with the following structure:
1.  **Input Layer:** Matches the vocabulary size.
2.  **Hidden Layers:** Two fully connected layers (8 neurons each) with generic activation.
3.  **Output Layer:** Softmax activation mapped to intent classes.

### **How to Run**
Since this project uses legacy TensorFlow libraries (`tflearn`), it is recommended to run this in a virtual environment.

1.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
2.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
3.  **Execution:** Run the cells sequentially to:
    * Load and preprocess `intents.json`.
    * Train the DNN model.
    * Engage with the chat interface at the bottom of the notebook.

### **Sample Interaction**
> **User:** "I'm feeling stressed."
> **Bot:** "If you're feeling overwhelmed, try taking a few deep breaths. I'm here to listen."

---
*Note: This project serves as a foundational study in NLP pipelines and neural network architecture design.*