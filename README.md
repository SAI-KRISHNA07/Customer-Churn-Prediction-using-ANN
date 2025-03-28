# Customer-Churn-Prediction-using-ANN
This project is designed to predict customer churn for a sample bank using a deep learning model. The model is built with TensorFlow/Keras and deployed as a Streamlit web application.

Table of Contents
Overview

Dataset

Model

Installation

Usage

Web Application

Results

Contributing

License

Overview
Customer churn is a significant challenge for banks and financial institutions. This project applies machine learning and deep learning techniques to predict whether a customer is likely to leave the bank. The model is trained on a sample dataset and integrated into a web-based application, allowing users to input customer details and obtain a churn probability prediction.

Dataset
The dataset (Churn_Modelling.csv) contains customer information, including:

Demographic details: Geography, gender, age, estimated salary

Account details: Credit score, tenure, balance, number of products, credit card ownership, and active membership status

Target variable: Whether the customer has churned or not

Model
The predictive model is a deep neural network built with TensorFlow/Keras. The input features are preprocessed using label encoding, one-hot encoding, and standard scaling. The model provides a probability score indicating the likelihood of customer churn.

Installation
To set up and run this project locally, follow these steps:

Clone the repository

bash
Copy
Edit
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
Create a virtual environment (optional but recommended)

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the application

bash
Copy
Edit
streamlit run app.py
Usage
Open the web application in a browser.

Enter the required customer details in the provided input fields.

The model will analyze the data and provide a churn probability score.

If the probability is greater than 0.5, the model predicts that the customer is likely to churn.

Web Application
The application is built using Streamlit and provides:

A user-friendly interface for entering customer data

Real-time predictions using the trained deep learning model

A clear display of the churn probability and its interpretation

Results
The model delivers an accurate prediction of customer churn, allowing banks to take proactive measures to retain customers. By leveraging these insights, financial institutions can improve customer satisfaction and reduce churn rates.

Contributing
Contributions to this project are welcome. If you would like to enhance the model or improve the application, feel free to fork the repository and submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.
