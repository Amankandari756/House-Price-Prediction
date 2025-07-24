# 🏡 House Price Prediction using Machine Learning

This project predicts house prices using the California housing dataset and machine learning models. It includes data preprocessing pipelines, model training, and prediction with outputs saved in CSV format.

## 📁 Files Included

- `main.py`: Final script to train the model or make predictions
- `main_old.py`: Script comparing models (Linear Regression, Decision Tree, Random Forest)
- `housing.csv`: Dataset containing housing features and prices
- `input.csv`: Input file for new predictions
- `output.csv`: Prediction results with house prices
- `model.pkl`: Saved trained Random Forest model
- `pipeline.pkl`: Saved preprocessing pipeline

## 🔧 How It Works

- On the **first run**, the script:
  - Splits the data using stratified sampling
  - Builds a pipeline for preprocessing
  - Trains a Random Forest model
  - Saves the model and pipeline
  - Generates `input.csv` for testing

- On **later runs**, it:
  - Loads the model and pipeline
  - Predicts prices for data in `input.csv`
  - Saves results to `output.csv`

## 🧠 Models Used

- Linear Regression (baseline)
- Decision Tree Regressor
- ✅ Random Forest Regressor (final deployed model)

## 🚀 Run the Project

### 1. First-Time Training

```bash
python main.py
