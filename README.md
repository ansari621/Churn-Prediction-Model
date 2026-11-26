# Customer Churn Prediction

A Streamlit app that uses an artificial neural network (ANN) to estimate a bank customer's probability of churning.

## Features

- Enter customer details and view a churn probability.
- Uses a trained Keras model, with scikit-learn encoders and scaler.

## Project files

- `app.py` — Streamlit application.
- `ann_classification.ipynb` — data preprocessing and model training.
- `churn_model.keras` — trained churn classifier.
- `scaler.pkl`, `label_encoder_gender.pkl`, `ohe_geo.pkl` — preprocessing artifacts required by the app.
- `requirements.txt` — Python dependencies.
- `Churn_Modelling.csv` — training data; not required to run the app.

The `.pkl` files must remain compatible with the scikit-learn version used to load them. The model artifacts were generated with Python 3.13.

## Run locally

From the project directory, create and activate a virtual environment, then install dependencies:

```powershell
py -3.13 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python -m streamlit run app.py
