# Text Summarization with Neural Networks

## Overview

This project presents an Automatic Text Summarization (ATS) system using transformer-based neural networks and semantic evaluation techniques. The objective of the project is to generate concise and meaningful summaries from lengthy textual documents while preserving contextual relevance and semantic integrity.

The project utilizes the BART transformer model for abstractive summarization and integrates Sentence-BERT (SBERT) based semantic similarity analysis to improve evaluation reliability beyond traditional lexical metrics such as ROUGE.

---

## Features

- Abstractive text summarization using BART
- Semantic consistency evaluation using SBERT
- ROUGE-1, ROUGE-2, and ROUGE-L evaluation
- Comparative analysis of summarization models
- Dataset preprocessing and tokenization
- Graphical visualization of evaluation metrics
- Hybrid lexical + semantic evaluation framework

---

## Technologies Used

- Python
- Natural Language Processing (NLP)
- Hugging Face Transformers
- SentenceTransformers (SBERT)
- Google Colab
- Matplotlib
- Pandas
- NumPy
- ROUGE-score Library

---

## Dataset

The project uses benchmark datasets for training and evaluation purposes.

- CNN/DailyMail Dataset
- DUC 2002 Dataset

The CNN/DailyMail dataset is loaded dynamically using the Hugging Face `datasets` library:

```python
from datasets import load_dataset
dataset = load_dataset("cnn_dailymail", "3.0.0")
---

## Methodology

The proposed workflow follows these steps:

1. Data Collection
2. Text Preprocessing
   - Tokenization
   - Stopword Removal
   - Lemmatization
   - Sentence Segmentation
3. BART-based Abstractive Summarization
4. ROUGE Evaluation
5. Semantic Similarity Analysis using SBERT
6. Comparative Performance Analysis

---

## Evaluation Metrics

### ROUGE Metrics
- ROUGE-1
- ROUGE-2
- ROUGE-L

### Semantic Evaluation
- SBERT Cosine Similarity

---

## Semantic Consistency Categories

| Similarity Score | Category |
|------------------|----------|
| 0.85 – 1.0 | Excellent |
| 0.75 – 0.85 | Good |
| 0.60 – 0.75 | Average |
| Below 0.60 | Poor |

Safe semantic threshold: **0.75**

---

## Results

| Metric | Score |
|--------|-------|
| ROUGE-1 | 0.72 |
| ROUGE-2 | 0.48 |
| ROUGE-L | 0.69 |
| SBERT Similarity | 0.86 |

The experimental results demonstrate that semantic evaluation provides a more reliable assessment of summary quality compared to lexical overlap alone.

---

## Comparative Analysis

The proposed hybrid model was compared with traditional and transformer-based summarization approaches such as:
- TextRank
- Seq2Seq
- CNN-based Models
- BART
- PEGASUS

The proposed model achieved superior semantic consistency and contextual understanding.

---

## Visualizations Included

- Dataset Distribution Graph
- ROUGE Evaluation Graph
- Semantic Similarity Comparison
- Comparative Analysis Graph
- Workflow Architecture Diagram

---

## Future Scope

- Multilingual Text Summarization
- Legal and Medical Document Summarization
- Human Evaluation Integration
- Reinforcement Learning-based Summarization
- Hallucination Reduction Techniques
- Real-time Summarization Systems

---

## Contributors

- Simran Jha
- Amandeep Verma
- Vishal Tripathi

Special thanks to our faculty mentor/teacher for their valuable guidance and continuous support throughout the project.

---

## Conclusion

This project demonstrates that combining transformer-based summarization with semantic evaluation techniques significantly improves summary quality, contextual relevance, and semantic consistency. The integration of SBERT with traditional ROUGE metrics provides a more comprehensive and reliable evaluation framework for modern text summarization systems.

---

## References

1. A. Nenkova and K. McKeown, “Automatic Summarization,” Foundations and Trends in Information Retrieval, 2011.
2. R. Nallapati et al., “Abstractive Text Summarization using Sequence-to-Sequence RNNs,” 2016.
3. M. Lewis et al., “BART: Denoising Sequence-to-Sequence Pre-training,” ACL, 2020.
4. C.-Y. Lin, “ROUGE: A Package for Automatic Evaluation of Summaries,” 2004.
5. Z. Zhang et al., “PEGASUS: Pre-training with Extracted Gap-sentences,” 2020.

---
