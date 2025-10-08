# Movie Review Classifier for a Streaming Service

[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)](https://keras.io/)

A project to build a neural network that predicts if a movie is "good" based on the text of critic reviews, helping a streaming service make data-driven acquisition decisions. 🍅

---

## 📖 Project Overview

A major streaming service wants to automate its movie acquisition process. Since purchasing the rights to each film is expensive, they need a reliable way to predict a movie's quality before adding it to their catalog.

In this notebook, we take on the role of a machine learning engineer hired to solve this problem. We will build a neural network that acts as a "digital critic," analyzing written reviews to classify a movie as "good" or not.

This exercise focuses on two key areas:
1.  The fundamentals of converting raw **text data** into numerical features that a neural network can understand.
2.  The implementation of the Keras **Embedding Layer**, a powerful solution for working with categorical data like words.

---

## 🔬 Core Concepts

### From Text to Tensors
Before a neural network can learn from text, we must convert the words into numbers. Our pipeline will involve:
* **Tokenization:** Breaking down sentences into individual words or "tokens."
* **Vocabulary Building:** Creating a dictionary that maps each unique word to a specific integer.
* **Integer Encoding:** Converting each review into a sequence of integers.

### The Embedding Layer
A one-hot encoded vector for a large vocabulary is computationally inefficient. The **Embedding Layer** is an elegant solution to this problem.
* **What it is:** A trainable layer that maps each integer (representing a word) to a dense, low-dimensional vector.
* **Why it's powerful:** The network *learns* the optimal vector representation for each word during training. This means words with similar meanings will end up with similar vectors, capturing the semantic relationships in the text. It's a highly effective way to implement linear layers for categorical data. 

---

## 🎯 Learning Objectives

After completing this notebook, you will be able to:

1.  **Implement a Text Preprocessing Pipeline:** Convert raw text reviews into a format suitable for a neural network.
2.  **Understand and Use the Embedding Layer:** Explain its purpose and implement it in a Keras model to learn meaningful word representations.
3.  **Build a Text Classifier:** Construct, train, and evaluate a neural network for binary sentiment classification.
4.  **Solve a Business Problem:** Apply fundamental NLP techniques to address a realistic industry scenario.

---
