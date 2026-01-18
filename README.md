# IMDB Sentiment Analysis using RNN 🎬🧠

This project focuses on sentiment analysis of movie reviews from the IMDB dataset using a Recurrent Neural Network (RNN) implemented in PyTorch.

The goal is to classify each review as positive or negative based on its textual content.

## Dataset
- IMDB Movie Reviews Dataset
- Labels:
  - 0 → Negative
  - 1 → Positive
- Subset used:
  - 5,000 training samples
  - 5,000 testing samples

## Preprocessing
- Text tokenization using basic lowercase splitting
- Vocabulary built manually using `Counter`
- Special tokens:
  - `<pad>` for padding
  - `<unk>` for unknown words
- Sequences padded using `pad_sequence`

## Model Architecture
- Embedding Layer
- Recurrent Neural Network (RNN)
- Dropout Layer
- Fully Connected Layer

The model uses the final hidden state of the RNN for classification.

## Training
- Framework: PyTorch
- Optimizer: Adam
- Loss Function: Cross Entropy Loss
- Number of epochs: 3

## Evaluation
- Test Accuracy: **99.94%**

## Tools & Libraries
- Python
- PyTorch
- Hugging Face Datasets
- Google Colab

## Notes
This project demonstrates a full NLP pipeline, including custom preprocessing, dataset handling, and model implementation without relying on high-level NLP libraries.
