# Unemployment Analysis in India

## Project Overview

This is my second Data Science Internship project with Oasis Infobyte. This project explores unemployment trends in India between May 2019 and June 2020 using Python. The analysis focuses on regional differences, monthly unemployment trends and changes during the COVID-19 pandemic period.

The goal is to use data analysis and visualisation techniques to identify patterns and communicate meaningful insights from the dataset.

## Objectives

- Analyse average unemployment rates across Indian regions.
- Identify the 10 regions with the highest average unemployment rates.
- Examine monthly unemployment trends.
- Compare unemployment trends across selected regions.
- Investigate relationships between unemployment, estimated employment and labour force participation.
- Compare unemployment rates before and during the COVID-19 period.

## Tools and Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset

The analysis uses the **Unemployment in India** dataset obtained from Kaggle.

The dataset contains information about:
- Region
- Date
- Frequency
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Area (Rural or Urban)

The cleaned dataset contains 740 records covering May 2019 to June 2020.

## Project Structure

DataScience-Task2-UnemploymentAnalysis/
│
├── data/
│   └── raw/
│       ├── Unemployment in India.csv
│
├── screenshots/
│   ├── correlation_heatmap.png
│   ├── covid_comparison.png
│   ├── dataset_cleaning.png 
│   ├── monthly_trends.png 
│   ├── regional_trends.png 
│   └── top_10_regions.png
│
├── README.md
└── unemployment_analysis.ipynb


## Analysis Performed

1. **Data Loading and Cleaning**
   - I loaded the unemployment dataset using Pandas.
   - I inspected the dataset structure and data types.
   - I checked for missing values and duplicate records.
   - I removed completely empty rows and unnecessary spaces.
   - I converted the date column into datetime format.

2. **Exploratory Data Analysis**
   - I calculated average unemployment rates by region.
   - I identified the top 10 regions with the highest average unemployment rates.
   - I analysed monthly unemployment trends.
   - I compared unemployment trends across Haryana, Maharashtra and Tamil Nadu.

3. **Correlation Analysis**
   - I calculated correlations between unemployment rate, estimated employed and labour participation rate.
   - I used a heatmap to visualise the relationships.

4. **COVID-19 Period Comparison**
   - I compared average unemployment rates before March 2020 and from March 2020 onwards.
   - I visualised the differences using a bar chart.

## Key Findings

- Tripura recorded the highest average unemployment rate at approximately 28.35%.
- Haryana followed with an average unemployment rate of approximately 26.28%.
- Meghalaya recorded the lowest average unemployment rate at approximately 4.80%.
- Monthly unemployment increased sharply during April and May 2020.
- The average unemployment rate increased from 9.51% before March 2020 to 17.77% from March 2020 onwards.
- The correlation analysis showed weak linear relationships between the selected numerical variables.

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/lauramashudu-svg/OIBSIP.git
   ```

2. Navigate to the project folder:

   ```bash
   cd OIBSIP/DataScience-Task2-UnemploymentAnalysis
   ```

3. Install the required libraries if they are not already installed:

   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `unemployment_analysis.ipynb` and run the cells from top to bottom.

## Conclusion

The analysis highlights differences in unemployment across Indian regions and a substantial increase during the COVID-19 period. It demonstrates how Python libraries can be used to clean, explore, analyse and visualise real-world datasets.

## Internship

Oasis Infobyte — Data Science Internship

Task 2: Unemployment Analysis in India
