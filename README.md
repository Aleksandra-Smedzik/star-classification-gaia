# star-classification-gaia
Machine Learning project: Star spectral classification using Gaia DR3 data. Includes Decision Tree, Random Forest, LightGBM models optimized with Optuna.

## Project Overview

This project demonstrates the classification of stars into spectral classes (O, B, A, F, G, K, M) based on astrophysical parameters using data from the Gaia DR3 catalog. The goal was to build machine learning models that can accurately predict spectral classes while handling class imbalance challenges.

## Models used:

- Decision Tree Classifier (with Optuna hyperparameter optimization)

- Random Forest Classifier (with Optuna hyperparameter optimization)

- LightGBM Classifier (with Optuna hyperparameter optimization)

## Dataset

- Source: Gaia Archive DR3

- Records: ~28,000 stars after preprocessing

- Features: 9 numerical features (temperature, luminosity, parallax, etc.)

- Target: Spectral class (O, B, A, F, G, K, M)
  
## Technologies and Tools

- Python 
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- lightgbm
- imbalanced-learn (SMOTE, RandomOverSampler, RandomUnderSampler)
- Optuna

  ## Best Results
- **Best model:** Decision Tree Classifier optimized using Optuna
- **F1-score (macro):** 0.8857
- **Accuracy:** 96.7%
- Best balance between rare and dominant classes was achieved with Decision Tree + Optuna
- LightGBM achieved the highest accuracy but with slightly less balanced classification.

## Key Steps in the Project

- Exploratory Data Analysis (EDA)

- Feature selection and cleaning

- Class balancing strategies (undersampling, oversampling, SMOTE)

- Model building and evaluation

- Hyperparameter tuning with GridSearchCV and Optuna

- Results comparison

## How to Run

1. Clone this repository:
```bash
git clone https://github.com/Aleksandra-Smedzik/star-classification-gaia.git
```

2. Install dependencies:
pip install -r requirements.txt

3. Open star_classification_ML.ipynb in Jupyter Notebook or Google Colab

## License

MIT License

## Author

Created by Aleksandra Smędzik

[LinkedIn Profile](https://www.linkedin.com/in/aleksandra-smędzik)

This project was created as part of a postgraduate Data Science program and serves as a portfolio piece demonstrating skills in data analysis, machine learning, and hyperparameter optimization.

