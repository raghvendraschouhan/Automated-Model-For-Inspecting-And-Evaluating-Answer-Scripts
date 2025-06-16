# Automated Model for Inspecting and Evaluating Answer Scripts

## Overview
This project develops an automated system for evaluating descriptive and short-answer responses using advanced NLP and machine learning techniques. The system leverages semantic similarity between student answers and reference answers to predict correctness scores, employing models like BERT, T5, and Sentence-BERT alongside traditional ML algorithms. The best-performing model, SVR with RBF kernel, achieves an R² score of 0.605 and an F1-score of 0.81, demonstrating robust performance in grading tasks.

## Key Features
- **Preprocessing Pipeline**: Text normalization, punctuation removal, stopword filtering, and lemmatization.
- **Feature Representation**:  
  - Sparse: TF-IDF vectorization.  
  - Dense: BERT, T5, and Sentence-BERT embeddings.  
- **Models**: Logistic Regression, SVR (RBF), Random Forest, Gradient Boosting, and more.
- **Evaluation Metrics**: R² score, MSE, MAE, precision, recall, and F1-score.
- **User Interface**: Gradio-based web interface for real-time answer evaluation.

## Results
- **Best Model**: SVR (RBF) with Sentence-BERT embeddings (R² = 0.605, MSE = 0.0214, F1 = 0.81).
- **Comparative Performance**: Outperforms traditional TF-IDF and other ensemble methods.
- **Scalability**: Lightweight and deployable on standard cloud infrastructure.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/automated-answer-evaluation.git
   Dataset
The project leverages two publicly available benchmark datasets for training and evaluation:

Mohler Dataset: Focuses on Computer Science questions, providing question-answer pairs with human-labeled correctness scores.

SciEntsBank: Covers Biology and Physics domains, offering a diverse set of student responses for semantic similarity tasks.

Both datasets include:

Reference (model) answers.

Student responses with ground-truth labels (correct/incorrect).

Preprocessed JSON/CSV formats for easy integration.

For reproducibility, download links or preprocessing scripts can be found in data/README.md.



   
