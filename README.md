# Fake News Detection – README

## Project Overview
This repository contains a complete pipeline for detecting fake news articles using Natural Language Processing (NLP) and supervised machine learning. The goal is to classify news articles as **FAKE** or **REAL** based on semantic content rather than shallow keyword matching.

## Repository Structure
- `notebooks/`: Jupyter notebooks for data exploration, preprocessing, modeling, and evaluation.
- `data/`: Contains training and validation datasets.
- `models/`: Saved model files (Logistic Regression, Decision Tree, Random Forest).
- `figures/`: Visualizations including n-gram plots, word distributions, and confusion matrices.
- `report/`: Word-ready project report with embedded figure placeholders.

## Methodology
1. **Data Loading & Cleaning**: Handled nulls and ensured consistent formatting.
2. **Text Preprocessing**: Tokenization, stopword removal, lemmatization.
3. **Exploratory Data Analysis**: N-gram analysis, word frequency plots, character length distributions.
4. **Feature Engineering**: Used pretrained Word2Vec embeddings to create document vectors.
5. **Model Training**: Trained Logistic Regression, Decision Tree, and Random Forest classifiers.
6. **Evaluation**: Compared models using Accuracy, Precision, Recall, F1-score, and Confusion Matrix.

## Key Results
| Model              | Accuracy | Precision (FAKE) | Recall (FAKE) | F1 (FAKE) |
|-------------------|----------|------------------|---------------|-----------|
| Logistic Regression | 0.90     | 0.91             | 0.90          | 0.90      |
| Decision Tree       | 0.82     | 0.82             | 0.85          | 0.83      |
| Random Forest       | 0.90     | 0.90             | 0.92          | 0.91      |

- **Best Model**: Random Forest  
- **Priority Metric**: F1-score for FAKE class

## Observations
- FAKE news uses emotionally charged, repetitive language.
- REAL news is more fact-based and lexically diverse.
- Semantic embeddings improve generalization across writing styles.

## Requirements
```bash
!pip install --upgrade numpy==1.26.4
!pip install --upgrade pandas==2.2.2
!pip install --upgrade nltk==3.9.1
!pip install --upgrade spacy==3.7.5
!pip install --upgrade scipy==1.12
!pip install --upgrade pydantic==2.10.5
!pip install wordcloud==1.9.4
!python -m spacy download en_core_web_sm
```
## Contact
Created by [@karthikjuluru] [@sharma-kashish] - feel free to contact!
