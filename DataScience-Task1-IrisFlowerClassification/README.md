# Iris Flower Classification

## Project Overview

This project uses machine learning to classify Iris flowers into three species: Setosa, Versicolor, and Virginica. The classification is based on four measurements: sepal length, sepal width, petal length, and petal width.

The project was completed as part of the Oasis Infobyte Data Science Internship.

## Project Structure

DataScience-Task1-IrisFlowerClassification/
│
├── iris_classification.ipynb
├── README.md
└── screenshots/
    ├── iris_scatter_plot.png
    ├── iris_box_plots.png
    └── model_comparison.png


## Project Objectives

- Explore and understand the Iris dataset.
- Perform exploratory data analysis (EDA).
- Visualise differences between flower species.
- Prepare training and testing datasets.
- Train and evaluate classification models.
- Compare model performance and identify the best-performing model.

## Dataset

The Iris dataset was loaded using `sklearn.datasets.load_iris()` from Scikit-learn.

- Total samples: 150
- Numerical features: 4
- Target classes: 3
- Missing values: 0

### Features

- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

### Target Classes

- Setosa
- Versicolor
- Virginica

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Scikit-learn

## Methodology

### 1. Data Loading and Exploration

Loaded the Iris dataset and converted it into a Pandas DataFrame. Examined its dimensions, data types, missing values, and descriptive statistics.

### 2. Data Visualisation

Created a scatter plot comparing petal length and petal width, along with four box plots to compare feature distributions across the species.

The visualisations showed that Setosa was clearly separated by its petal measurements, while Versicolor and Virginica showed some overlap.

### 3. Data Preparation

Separated the four flower measurements into features (`X`) and the species labels into the target (`y`).

Split the data into 80% training data and 20% testing data, using stratification to preserve the class proportions.

### 4. Model Training and Evaluation

Trained and evaluated two classification algorithms:

- Logistic Regression
- K-Nearest Neighbors (KNN), using five neighbours

Evaluated the models using accuracy, confusion matrices, precision, recall, and F1-scores.

## Results

| Model | Test Accuracy |
|---|---:|
| Logistic Regression | 96.67% |
| K-Nearest Neighbors | 100.00% |

KNN achieved the highest test accuracy, correctly classifying all 30 test samples. Logistic Regression correctly classified 29 out of 30 samples.

KNN was selected as the best-performing model for this experiment based on test accuracy. The results are based on a single train-test split and do not guarantee the same performance on all unseen data.

## Conclusion

This project demonstrated how exploratory data analysis, visualisation, data preparation, and supervised machine learning can be used to classify Iris flowers.

Both models performed well, with KNN achieving 100% accuracy on the test set and Logistic Regression achieving 96.67%.

Further evaluation using cross-validation could help assess how consistently the models generalise to unseen data.

## Project Files

- `iris_classification.ipynb` — Jupyter Notebook containing the analysis, visualisations, model training, and evaluation.

## How to Run

1. Clone or download the repository.
2. Install Python and the required libraries.
3. Open the notebook in Jupyter Notebook or Visual Studio Code.
4. Run the notebook cells from top to bottom.

Install the required libraries with:

```bash
pip install pandas scikit-learn matplotlib seaborn jupyter ipykernel
```

## Internship

Oasis Infobyte — Data Science Internship

Task 1: Iris Flower Classification