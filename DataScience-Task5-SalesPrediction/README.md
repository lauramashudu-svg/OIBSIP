# Sales Prediction Using Python

## Project Overview

This project focuses on predicting product sales using machine learning regression techniques.

The model uses advertising expenditure across three marketing channels:
- TV
- Radio
- Newspaper

The objective is to analyse how advertising expenditure relates to product sales and build models that can predict sales based on advertising budgets.

## Dataset

The project uses the Advertising dataset downloaded from Kaggle.

**Dataset source:** [Advertising Sales Prediction Dataset – Kaggle](https://www.kaggle.com/datasets/bumba5341/advertisingcsv)

The dataset contains 200 records and four columns:

| Column | Description |
|---|---|
| TV | TV advertising expenditure |
| Radio | Radio advertising expenditure |
| Newspaper | Newspaper advertising expenditure |
| Sales | Product sales |

The unnecessary index column was removed during data cleaning.

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Workflow

The following steps were completed:

1. Imported the required Python libraries.
2. Loaded and inspected the dataset.
3. Removed the unnecessary index column.
4. Checked for missing values and duplicate records.
5. Performed descriptive statistical analysis.
6. Conducted Exploratory Data Analysis (EDA).
7. Created pairplots and individual scatter plots.
8. Analysed correlations using a heatmap.
9. Split the dataset into training and testing sets.
10. Trained Linear Regression and Random Forest Regression models.
11. Evaluated both models using MAE, RMSE and R².
12. Created a residual plot for the best-performing model.
13. Analysed advertising channel importance.
14. Compared model performance and documented the findings.

## Model Performance

Two regression models were trained and evaluated.

| Metric | Linear Regression | Random Forest |
|---|---:|---:|
| MAE | 1.4608 | 0.6203 |
| RMSE | 1.7816 | 0.7687 |
| R² Score | 0.8994 | 0.9813 |

Random Forest Regression achieved better results across all three evaluation metrics.

It was therefore selected as the best-performing model.

## Feature Importance

The Random Forest model identified the following advertising channel importance scores:

| Advertising Channel | Importance |
|---|---:|
| TV | 62.48% |
| Radio | 36.22% |
| Newspaper | 1.30% |

TV advertising was the most important predictor of sales, followed by Radio and Newspaper advertising.

These scores represent the model's predictive feature importance, not proof of direct causation.

## Conclusion

The project demonstrated how machine learning regression models can be used to predict product sales based on advertising expenditure.

Random Forest Regression achieved the best performance, with an R² score of 0.9813.

The feature importance analysis showed that TV advertising contributed the most to the model's predictions.

Overall, the project provided practical experience in data cleaning, exploratory data analysis, data visualisation, regression modelling and model evaluation.

## How to Run the Project

1. Clone or download the repository.
2. Open the Task 5 project folder.
3. Install the required libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

4. Open Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `sales_prediction.ipynb` and run the notebook cells.

## Project Structure


DataScience-Task5-SalesPrediction/
│
├── data/
│   └── raw/
│       └── Advertising.csv
│
├── screenshots/
│
├── README.md
│
└── sales_prediction.ipynb


