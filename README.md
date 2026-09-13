# Ford Car Price Prediction

A Linear Regression project that predicts the resale price of used Ford cars
based on features such as model, year, mileage, transmission, fuel type,
engine size, tax, and mpg.

## Overview

This notebook walks through a complete, end-to-end regression workflow:

1. **Data loading & inspection** — shape, types, missing values, summary stats
2. **Exploratory Data Analysis (EDA)** — price distribution, correlations, and
   relationships between price and each feature (year, mileage, engine size,
   transmission, fuel type, model, tax, mpg)
3. **Feature encoding** — two parallel approaches are compared:
   - **One-Hot Encoding** for categorical variables
   - **Label Encoding** for categorical variables
4. **Feature scaling** — `StandardScaler` applied to numeric features
5. **Model training** — `LinearRegression` from scikit-learn, trained on both
   encoded feature sets
6. **Evaluation** — R² and Adjusted R² for each approach, to see which
   encoding strategy performs better

## Dataset

This project uses the [Ford Car Price Prediction dataset](https://www.kaggle.com/datasets/adhurimquku/ford-car-price-prediction)
(`ford.csv`) from Kaggle, containing ~18,000 used Ford car listings with the
following columns:

| Column | Description |
|---|---|
| `model` | Car model (e.g. Fiesta, Focus) |
| `year` | Registration year |
| `price` | Sale price (target variable) |
| `transmission` | Manual / Automatic / Semi-Auto |
| `mileage` | Distance driven (miles) |
| `fuelType` | Petrol / Diesel / Hybrid / Electric |
| `tax` | Road tax band |
| `mpg` | Fuel efficiency (miles per gallon) |
| `engineSize` | Engine displacement (litres) |

## Getting Started

### Prerequisites

- Python 3.9+
- Jupyter Notebook or JupyterLab

### Installation

```bash
git clone https://github.com/Lovelydehar3/ford-car-price-prediction.git
cd ford-car-price-prediction
pip install -r requirements.txt
```

### Dataset Setup

1. Download `ford.csv` from [Kaggle](https://www.kaggle.com/datasets/adhurimquku/ford-car-price-prediction)
2. Place it in a `data/` folder in the project root (or update the
   `DATA_PATH` variable in the notebook)

### Running the Notebook

```bash
jupyter notebook ford-car-price-prediction.ipynb
```

Run all cells top to bottom. The final section prints R² and Adjusted R²
for both the one-hot encoded and label-encoded models so you can compare
their performance.

## Project Structure

```
.
├── ford-car-price-prediction.ipynb   # Main analysis & modeling notebook
├── ford.csv                      # Dataset
├── requirements.txt                  # Python dependencies
└── README.md
```

## Results

The notebook trains two Linear Regression models — one on one-hot encoded
features, one on label-encoded features — and reports R² and Adjusted R²
for each, making it easy to see which categorical encoding strategy suits
this dataset best. Populate this section with your own numbers after
running the notebook.

## Tech Stack

- [pandas](https://pandas.pydata.org/) & [NumPy](https://numpy.org/) — data manipulation
- [Matplotlib](https://matplotlib.org/) & [Seaborn](https://seaborn.pydata.org/) — visualization
- [scikit-learn](https://scikit-learn.org/) — preprocessing, modeling, and evaluation

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Dataset by [adhurimquku on Kaggle](https://www.kaggle.com/datasets/adhurimquku/ford-car-price-prediction)
#
