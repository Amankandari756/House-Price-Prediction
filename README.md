California Housing Price Prediction
This project implements an end-to-end machine learning pipeline to predict median house values in California using the California housing dataset. It demonstrates data preprocessing, model training, and inference using scikit-learn and pandas.

Features
Data Loading & Splitting: Loads housing.csv and creates a stratified train/test split.

Data Preprocessing Pipeline: Uses scikit-learn's Pipeline and ColumnTransformer for:

Handling missing numerical values (SimpleImputer).

Scaling numerical features (StandardScaler).

One-hot encoding categorical features (OneHotEncoder).

Model Training: Trains a RandomForestRegressor model.

Model Persistence: Saves the trained model and preprocessing pipeline using joblib.

Inference: Loads the saved model/pipeline to make predictions on input.csv and saves results to output.csv.

Technologies Used
Python 3.x

pandas

numpy

scikit-learn

joblib

Files in this Project
housing.csv: Primary dataset.

main.py: Main script for training and inference.

main_old.py: Older script for model experimentation.

input.csv: Sample data for predictions (generated from test set).

output.csv: Prediction results.

model.pkl: (Generated) Trained RandomForestRegressor model.

pipeline.pkl: (Generated) Preprocessing pipeline.

How to Run
Ensure all files are in the same directory.

Install libraries:

pip install pandas numpy scikit-learn joblib

Run the script:

python main.py

First run: Model training, model.pkl, pipeline.pkl, and input.csv creation.

Subsequent runs: Inference on input.csv, results saved to output.csv.

Key Learnings
This project provided practical experience in:

Implementing robust data preprocessing.

Applying stratified sampling.

Building efficient ML pipelines.

Training and evaluating regression models (RandomForestRegressor).

Model persistence for deployment.

This project provided a comprehensive understanding of the end-to-end machine learning workflow.
