
# Credit Card Fraud Detection Frontend

This is a lightweight Streamlit web app that connects to a deployed FastAPI backend and provides a user-friendly interface for predicting fraudulent credit card transactions.




## About

The app allows users to enter transaction features like Time, Amount, and PCA-transformed values (V1 to V28), and it returns whether the transaction is fraudulent or not, along with the probability score.

This frontend interacts with a separately hosted backend API built using FastAPI, which serves a trained machine learning model for fraud detection.
## How it Works

The user inputs transaction details through the Streamlit interface. These values are sent as a JSON POST request to the FastAPI endpoint. The backend processes the input, applies the appropriate scaler, uses the trained model to predict, and returns a response with the prediction and confidence score.
## Files in this Repo

*streamlit_app.py* : The main Streamlit app script.

*requirement.txt* : Python dependencies for deploying the app on platforms like Streamlit Cloud.

*.gitignore* : Specifies files and folders to be excluded from version control (e.g., virtual environments, system files).

*LICENSE* : The license for this repository.
## Related Repo

This frontend works with the API backend repository:
https://github.com/shubhashishgari/credit-card-fraud-detection-api 