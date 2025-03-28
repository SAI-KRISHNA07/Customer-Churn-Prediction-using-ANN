# Customer-Churn-Prediction-using-ANN

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)  
[![Streamlit](https://img.shields.io/badge/Streamlit-App-red.svg)](https://streamlit.io/)  

## Project Overview  
This project predicts **customer churn** for a sample bank using a deep learning model built with TensorFlow/Keras. The model analyzes customer attributes (such as credit score, age, and balance) and provides a **churn probability score**.

### **The project includes:**  
✔️ A **trained neural network** for prediction  
✔️ **Data preprocessing** using encoding and scaling  
✔️ A **Streamlit web app** for user interaction  
✔️ A structured **dataset for training and evaluation**  

---

## Table of Contents  
- [Dataset](#-dataset)  
- [Project Structure](#-project-structure)  
- [Installation](#-installation)  
- [Usage](#-usage)  
- [Web Application](#-web-application)  
- [Results](#-results)  
- [Contributing](#-contributing)  
- [License](#-license)  

---

## Dataset  
The dataset used is **`Churn_Modelling.csv`**, which contains:  

- **Customer demographics**: Geography, gender, age  
- **Financial details**: Credit score, balance, estimated salary  
- **Account details**: Number of products, tenure, active membership status  
- **Target variable**: Whether the customer has churned  

| Feature         | Description |
|----------------|-------------|
| `CreditScore`  | Customer’s credit score |
| `Geography`    | Country of the customer |
| `Gender`       | Male or Female |
| `Age`          | Customer’s age |
| `Balance`      | Account balance |
| `NumOfProducts` | Number of bank products used |
| `HasCrCard`    | Whether the customer has a credit card (0 or 1) |
| `IsActiveMember` | Whether the customer is active (0 or 1) |
| `EstimatedSalary` | Customer’s estimated salary |
| `Exited`       | Churn label (1 = churned, 0 = retained) |

---

## Project Structure  
```
customer-churn-prediction/
│── app.py                  # Streamlit web app
│── ann.ipynb               # Jupyter Notebook for model training
│── Churn_Modelling.csv     # Dataset
│── model.h5                # Saved deep learning model
│── scaler.pkl              # StandardScaler for input normalization
│── label_encoder_gender.pkl # Encoded gender values
│── onehot_encoder_geo.pkl  # Encoded geographical values
│── README.md               # Documentation
│── requirements.txt        # Required libraries
```

---

## ⚙ Installation  
To run this project locally, follow these steps:  

### **1️ Clone the repository**  
```bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
```

### **2️ Create a virtual environment (optional but recommended)**  
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### **3️ Install dependencies**  
```bash
pip install -r requirements.txt
```

### **4️ Run the web application**  
```bash
streamlit run app.py
```

---

## Usage  
1. Open the **Streamlit web app**.  
2. Enter customer details using the provided input fields.  
3. Click **"Predict"** to get the **churn probability score**.  
4. If the probability is **greater than 0.5**, the customer is predicted to churn.  

---

## Web Application  
The project includes a **Streamlit-based web interface** for easy interaction.  

🔹 **Dropdowns and sliders** for customer data input  
🔹 **Real-time predictions** using the trained deep learning model  
🔹 **Automated preprocessing** for categorical and numerical inputs  
🔹 **Clear visualization** of the churn probability  

### **Example Prediction Output**  
```txt
Churn Probability: 0.72

The customer is likely to churn.
```

---

## Results  
The deep learning model achieves a **high prediction accuracy** for customer churn. Some key insights:  
✔️ Customers with **low credit scores and high balances** have a higher churn risk.  
✔️ **Active members** and those with **multiple products** are less likely to churn.  
✔️ The **model is effective** in identifying at-risk customers.  

---

## Contributing  
Contributions are welcome! To contribute:  
1. **Fork the repository**.  
2. Create a new branch:  
   ```bash
   git checkout -b feature-branch
   ```
3. Make improvements and **commit changes**.  
   ```bash
   git commit -m "Improved model performance"
   ```
4. Push changes and create a **pull request**.  

---

## License  
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.  

---

### 🔗 Useful Links  
📌 **Streamlit Documentation** – [https://docs.streamlit.io/](https://docs.streamlit.io/)  
📌 **TensorFlow Documentation** – [https://www.tensorflow.org/](https://www.tensorflow.org/)  

---

