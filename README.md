# Next-Word-Predictor-WikiText2
Neural Trigram Language Model (PyTorch)
📌 Overview

This project implements a Neural Trigram Language Model using PyTorch.
The model learns to predict the next word in a sequence based on the previous two words, using word embeddings and a feed-forward neural network.

The project demonstrates core concepts in Natural Language Processing (NLP), including:

Language Modeling
Word Embeddings
Cross-Entropy Loss
Accuracy and Perplexity evaluation
🧠 Model Architecture

The model consists of:

Embedding Layer to convert word indices into dense vectors
Fully Connected Hidden Layer with ReLU activation
Output Layer that predicts a probability distribution over the vocabulary

Input: Two consecutive words
Output: Predicted next word
⚙️ Training Details
Vocabulary size: Top N most frequent words (+ <unk>, <pad>)
Embedding dimension: 64
Hidden dimension: 128
Optimizer: Adam
Loss Function: CrossEntropyLoss
Training approach: Trigram-based prediction
📊 Evaluation Metrics

The model is evaluated using:

🔹 Accuracy

Measures how often the model predicts the correct next word.

🔹 Perplexity

A standard metric for language models that measures how “confused” the model is when predicting the next word.

Lower perplexity indicates better performance.

Perplexity=e
Cross Entropy Loss
🔍 Example Prediction
Input:  "in the"
Output: ["world", "city", "case", ...]
🚀 Future Improvements

Possible enhancements include:

Mini-batch training for better stability
Larger context size (4-gram or 5-gram)
Replacing the feed-forward model with LSTM or Transformer
Vocabulary pruning and better text preprocessing
🛠 Technologies Used
Python
PyTorch
Natural Language Processing (NLP)
