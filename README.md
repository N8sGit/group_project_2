![Wine Quality Predictor](images/wine_quality_predictor.jpg)

## Overview

The Wine Quality Predictor is a machine learning project aimed at predicting the quality of Vinho Verde wine (both Red and White) from Portugal's northwest region. The project encompasses data sourcing, transformation, exploratory data analysis, model training, and visualization.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Data](#data)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Model Training](#model-training)
7. [Evaluation](#evaluation)
8. [Results](#results)
9. [License](#license)
10. [Team](#team)
11. [References](#references)

## Introduction

This project explored using machine learning to predict the quality of Vinho Verde wine from Portugal's northwest region. It involved project ideation, data sourcing, and transformation using Excel and Python to create a usable dataframe and CSV file. Power BI was used to gather insights on the dataset and assess the feasibility of our hypothesis, followed by formatting and exploratory data analysis in Python.

## Features

- Predicts wine quality based on chemical properties
- Supports both red and white wine data
- Provides insights into which factors most influence wine quality

## Data

The dataset used in this project was sourced from Kaggle and includes two CSV files: `wine_data_white.csv` and `wine_data_red.csv`. These were combined into a single file, `wine_data_both.csv`.

The dataset contains the following columns:

- `Index`
- `fixed acidity`
- `volatile acidity`
- `citric acid`
- `residual sugar`
- `chlorides`
- `free sulfur dioxide`
- `total sulfur dioxide`
- `density`
- `pH`
- `sulphates`
- `alcohol`
- `quality`
- `Wine` (Type of wine: Red or White)

## Installation

To run this project locally, you'll need Python and additional libraries installed. Use the following command to install the required libraries:

```bash
pip install pandas numpy scikit-learn imbalanced-learn matplotlib statsmodels
```

## Usage

1. **Clone the repository:**

```bash
git clone git@github.com:N8sGit/group_project_2.git
cd group_project_2
```

## Methodology 

2. ***Data Preparation***  
* Synthetic data generation to correct extreme imbalances between the minority class (n=5) and majority class (n=2836).  
* Binning to correct for extreme data imbalances (merging the minority classes at the ends of the distribution)
* Noise elimination: Uses IsolationForest model to detect and remove outliers. 
* Feature selection: Uses Lasso Regression, mean squared error calculation, and variance inflation factor to detect the most what features don’t contribute to or distort the model. 

3. ***Model Selection***
* Hyper-parameter tuning 
* RandomizedSearchCV to traverse a randomized subspace 
* Manual experimentation and trial and error to determine that RandomForestClassifier is the most reliably performing algorithm 

4. ***Model Validation***
* Cross Validation to confirm consistency of results across several randomized folds
* A/B testing against raw data to contrast with our changes 

5.  ***Model Interpretation***
* Feature Importance comparison and analysis  

## Results

The project involved extensive exploratory data analysis, including descriptive statistics, correlation heatmaps, box plots, histograms, violin plots, and p-value analysis (which did not provide significant results). Key steps included:

- Analyzing the 'Quality' variable for correlation and removing highly correlated variables (free sulfur dioxide and density).
- Reviewing the distribution of all variables and removing outliers for model training.

### Describe Chart
![Describe chart](images/describe_chart.png)

### Correlation Heatmap
![Correlation Heatmap](images/correlation_heatmap.png)

### Box Plot
![Box Plot](images/box_plot.png)

### Histogram Charts
![Histogram Chart](images/histogram_chart.png)

### Violinplots
![Violinplots](images/violion_plot.png)

The key takeaway is that alcohol is the best predictor for high-quality wine using a Random Forest Model. Detailed results and visualizations can be found in the `results/` directory.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Team

- Elizabeth Arias
- Dawn Kim
- Christian Leon
- Nathan Anecone
- Ian Cody
- Kyle Prudente

## References

- Kaggle.com: P. Cortez, A. Cerdeira, F. Almeida, T. Matos, and J. Reis. Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009.