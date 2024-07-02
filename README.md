![Wine Quality Predictor](wine_quality_predictor.jpg)


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
9. [Contributing](#contributing)
10. [License](#license)
11. [Team](#team)
12. [References](#references)

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
pip install -r requirements.txt
```

## Usage

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/wine-quality-predictor.git
cd wine-quality-predictor
```

2. **Prepare the data:**

Place your wine dataset CSV files (`wine_data_white.csv`, `wine_data_red.csv`, `wine_data_both.csv`) in the `data/` directory.

3. **Run the prediction script:**

```bash
python predict.py --input data/wine_data_both.csv
```

## Model Training

To train the model, follow these steps:

1. **Preprocess the data:**

```bash
python preprocess.py --input data/wine_data_both.csv --output data/processed_wine_data.csv
```

2. **Train the model:**

```bash
python train.py --input data/processed_wine_data.csv --output models/wine_quality_model.pkl
```

## Evaluation

Evaluate the model's performance using the test dataset:

```bash
python evaluate.py --model models/wine_quality_model.pkl --input data/test_wine_data.csv
```

## Results

The project involved extensive exploratory data analysis, including descriptive statistics, correlation heatmaps, box plots, histograms, violin plots, and p-value analysis (which did not provide significant results). Key steps included:

## Describe Chart

## Correlation Heatmap

## Box Plot

## Histogram Charts

## Violinplots

Analyzing the 'Quality' variable for correlation and removing highly correlated variables (free sulfur dioxide and density).
Reviewing the distribution of all variables and removing outliers for model training.
The key takeaway is that alcohol is the best predictor for high-quality wine using a Random Forest Model. Detailed results and visualizations can be found in the results/ directory.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes and commit (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a new Pull Request

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

---

Feel free to reach out if you have any questions or need further assistance. Enjoy predicting wine quality!

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to reach out if you have any questions or need further assistance. Enjoy predicting wine quality!
