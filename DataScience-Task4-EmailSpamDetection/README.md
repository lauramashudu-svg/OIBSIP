# Task 4: Email Spam Detection with Machine Learning

## Project Overview

This project focuses on developing a machine learning classification system that identifies spam and legitimate messages using Natural Language Processing (NLP).

The project uses the SMS Spam Collection dataset to train and evaluate two machine learning algorithms: Multinomial Naive Bayes and Logistic Regression.

Although the task focuses on email spam detection, the selected dataset contains SMS messages labelled as spam or ham.

## Objectives

- Load and explore a text classification dataset.
- Clean and preprocess text messages.
- Convert text into numerical features using TF-IDF.
- Train two machine learning classification models.
- Evaluate model performance using classification metrics.
- Compare the results and identify the better-performing model.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- NLTK
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset

**Dataset:** SMS Spam Collection

The dataset contains 5,572 original messages classified into two categories:

- **Ham:** Legitimate messages.
- **Spam:** Unwanted messages.

After removing unnecessary columns and 403 duplicate records, 5,169 unique messages remained.

## Project Structure


DataScience-Task4-EmailSpamDetection/
│
├── data/
│   └── raw/
│       └── spam.csv
│
├── screenshots/
│   ├── 01_dataset_overview.png
│   ├── 02_data_cleaning.png
│   ├── 03_class_distribution.png
│   ├── 04_text_preprocessing.png
│   ├── 05_tfidf_features.png
│   ├── 06_model_training.png
│   ├── 07_model_evaluation.png
│   └── 08_project_conclusion.png
│
├── README.md
│
└── spam_detection.ipynb


## Data Preprocessing

The following preprocessing steps were performed:

1. Converted messages to lowercase.
2. Removed punctuation and numbers.
3. Removed common English stopwords.
4. Removed duplicate messages.
5. Prepared the cleaned text for feature extraction.

## Feature Extraction

TF-IDF (Term Frequency-Inverse Document Frequency) was used to convert text messages into numerical features.

The vectorizer learned 6,608 features from the training dataset.

## Machine Learning Models

Two classification algorithms were trained:

1. Multinomial Naive Bayes
2. Logistic Regression

The dataset was divided into:
- 80% training data.
- 20% testing data.

Stratified sampling was used to maintain the class distribution.

## Model Evaluation Results

| Evaluation Metric | Multinomial Naive Bayes | Logistic Regression |
|---|---:|---:|
| Accuracy | 96.62% | 95.94% |
| Precision | 98.98% | 98.90% |
| Recall | 74.05% | 68.70% |
| F1-score | 84.72% | 81.08% |

## Confusion Matrix Analysis

**Multinomial Naive Bayes:**
- True Negatives: 902
- False Positives: 1
- False Negatives: 34
- True Positives: 97

**Logistic Regression:**
- True Negatives: 902
- False Positives: 1
- False Negatives: 41
- True Positives: 90

## Conclusion

Multinomial Naive Bayes achieved the best overall performance, with an accuracy of 96.62% and an F1-score of 84.72%.

It also achieved a higher spam recall than Logistic Regression, identifying more actual spam messages.

Based on the evaluation results, Multinomial Naive Bayes was selected as the better-performing model for this dataset.

## How to Run the Project

1. Clone or download the repository.
2. Install the required Python libraries.
3. Open the project