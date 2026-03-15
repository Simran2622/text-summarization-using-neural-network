# Text Summarization using Neural Network

This project implements an abstractive text summarization system using a transformer-based neural network model.

## Model
BART (facebook/bart-large-cnn)

## Dataset
CNN/DailyMail dataset

Dataset subset used for experiments:
- Training: 2000 samples
- Validation: 500 samples
- Testing: 500 samples

## Evaluation Metric
ROUGE metrics were used to evaluate summarization quality.

Results obtained:
- ROUGE-1 ≈ 0.38
- ROUGE-2 ≈ 0.18
- ROUGE-L ≈ 0.29

## Project Pipeline
Article → Tokenization → BART Neural Network → Generated Summary → ROUGE Evaluation

## Implementation Notebook
notebooks/text_summarization_final.ipynb

This project demonstrates neural text summarization using transformer models.
