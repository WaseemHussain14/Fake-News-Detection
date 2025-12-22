# Fake News Detection Using ML & NLP

This project aims to detect fake news articles using Machine Learning and Natural Language Processing techniques.

The project will be deployed using Streamlit,

## Project Overview

Fake news poses a significant challenge in the digital era by spreading misinformation at scale.

This project addresses the problem by building a supervised machine learning pipeline that
classifies news articles as real or fake based on their textual content.

The system includes data preprocessing, TF-IDF based feature extraction, and classification
models, followed by deployment as an interactive web application.

## Dataset

The dataset used in this project is the Fake and Real News Dataset from Kaggle.

Link: https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset

Download the dataset and place `Fake.csv` and `True.csv` inside a `data/` folder
at the project root.

## Project Structure

```text
Fake-News-Detection/
│
├── data/                # Dataset files (ignored by git)
├── artifacts/           # Saved models and vectorizers (ignored by git)
├── notebooks/           # Jupyter notebooks
│   ├── 01datapreprocessing.ipynb
│   ├── 02_tfidf_vectorization.ipynb
│   └── 03_model_training.ipynb
├── README.md
├── .gitignore
```
## Model Training and Results

Multiple machine learning models were trained and evaluated using TF-IDF feature representations to identify the most effective classifier for fake news detection.

### Models Evaluated
- Logistic Regression
- Naive Bayes (Multinomial)

### Performance Summary

| Model | Accuracy | F1-Score |
|------|----------|----------|
| Logistic Regression | ~98% | ~0.98 |
| Naive Bayes | ~93% | ~0.93 |

### Final Model Selection

Logistic Regression was selected as the final model due to its superior performance across precision, recall, and F1-score metrics.

Compared to Naive Bayes, it demonstrated stronger generalization and more consistent predictions across both classes, making it more suitable for deployment.
