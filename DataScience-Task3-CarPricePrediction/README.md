# Car Price Prediction with Machine Learning

## Project Overview

This is my second Data Science Internship project with **Oasis Infobyte**. This project uses machine learning regression techniques to predict the selling prices of used vehicles based on different vehicle characteristics.

## Objective

The objective is to build and evaluate regression models that estimate used vehicle selling prices using features such as:

- Vehicle brand
- Vehicle age
- Present price
- Kilometres driven
- Fuel type
- Seller type
- Transmission type
- Previous ownership

## Dataset

The project uses the **Vehicle Dataset from CarDekho**, provided by Nehal Birla on Kaggle.

The dataset contains information about used vehicles, including their selling prices, original prices, manufacturing years, fuel types and transmission types.

The dataset file used is `car data.csv`.

## Technologies and Libraries

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Project Workflow

1. I imported the required Python libraries.
2. I loaded and inspected the dataset.
3. I cleaned the data by removing duplicate records and standardising categorical values.
4. Performed feature engineering by extracting vehicle brands and calculating vehicle age.
5. I conducted Exploratory Data Analysis (EDA).
6. Encoded categorical features using One-Hot Encoding.
7. Split the dataset into training and testing sets.
8. Trained Linear Regression and Random Forest Regression models.
9. Evaluated both models using MAE, RMSE and R-squared.
10. Compared model performance and visualised the Linear Regression coefficients.

## Exploratory Data Analysis

The following visualisations were created:

- Distribution of vehicle selling prices.
- Selling prices by fuel type.
- Vehicle age versus selling price.
- Correlation heatmap of numerical features.

## Machine Learning Models

Two regression algorithms were trained:

- Linear Regression
- Random Forest Regression

### Model Evaluation Results

| Model             | MAE  | RMSE | R-squared |
|---                |---   |---   |---        |
| Linear Regression | 1.52 | 2.54 | 0.75      |
| Random Forest     | 1.42 | 3.49 | 0.53      |

*NB: Selling prices are expressed in Indian Rupees lakh(₹), following the dataset's original units.*

### Best Performing Model

Linear Regression performed better overall based on its lower RMSE and higher R-squared score.

Random Forest achieved a slightly lower MAE, showing that it had a smaller average absolute prediction error.

## Feature Importance

The Linear Regression coefficients were examined to identify features with relatively large influences on predictions.

Fuel type, transmission type and seller type appeared among the features with the largest absolute coefficients.

The coefficients were not standardised, so their magnitudes should be interpreted with caution.

## Project Structure

DataScience-Task3-CarPricePrediction/
│
├── data/
│   └── raw/
│       └── car data.csv
│
├── screenshots/
│   ├── data_cleaning.png
│   ├── dataset_overview.png
│   ├── exploratory_data_analysis.png
│   ├── model_evaluation.png
│   ├── model_heatmap.png
│   └── output.png
│   └── visual_analysis.png
│
├── car_price_prediction.ipynb
└── README.md


## How to Run the Project

1. Clone or download this repository.
2. Open the project folder in VS Code.
3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

4. Open `car_price_prediction.ipynb`.
5. Select a Python kernel.
6. Run all notebook cells.

## Conclusion

This project demonstrated how machine learning can be applied to used vehicle price prediction.

Data cleaning, feature engineering, visualisation and regression modelling were used to prepare and analyse the dataset.

Both Linear Regression and Random Forest were evaluated. Linear Regression achieved the better overall performance on the test dataset.

The project provided practical experience in data analysis, machine learning model development and model evaluation.

## Internship

Oasis Infobyte — Data Science Internship

Task 3: Car Price Prediction
