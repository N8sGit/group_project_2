# Wine Quality Predictor


## Overview

The Wine Quality Predictor is a machine learning project designed to predict the quality of wine based on its various chemical properties. By analyzing these properties, the model aims to provide a quality score for both red and white wines.

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

## Introduction

This project uses machine learning algorithms to analyze wine characteristics and predict their quality. The dataset includes various chemical properties of red and white wines, such as acidity, sugar content, pH levels, and more. By understanding these properties, the model can identify key factors that contribute to high-quality wine.

## Features

- Predicts wine quality based on chemical properties
- Supports both red and white wine data
- Provides insights into which factors most influence wine quality

## Data

The dataset used in this project contains the following columns:

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

To run this project locally, you'll need to have Python and some additional libraries installed. You can install the required libraries using the following command:

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

Place your wine dataset CSV files (`Wine_data_both.csv`, `Wine_data_red.csv`, `Wine_data_white.csv`) in the `data/` directory.

3. **Run the prediction script:**

```bash
python predict.py --input data/Wine_data_both.csv
```

## Model Training

To train the model, follow these steps:

1. **Preprocess the data:**

```bash
python preprocess.py --input data/Wine_data_both.csv --output data/processed_wine_data.csv
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

The model's performance metrics and insights into the most influential factors will be displayed after running the evaluation script. 

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to reach out if you have any questions or need further assistance. Enjoy predicting wine quality!
