# 📉 Customer Churn Prediction Model

A Machine Learning-based system to predict customer churn using classification techniques. This project includes both a **Streamlit Web App** for interaction and a **FastAPI backend** for real-time predictions.

---

## 🚀 Features

* Customer churn prediction using ML models
* Data preprocessing & feature engineering
* Model training & evaluation
* REST API using FastAPI
* Interactive dashboard using Streamlit
* Export predictions & performance metrics

---

## 📁 Project Structure

```
Customer-Churn-Prediction-Model/
│
├── api/
│   └── fastapi_app.py
│
├── data/
│   ├── telco_churn.csv
│   └── Telco-Customer-Churn.csv
│
├── models/
│   └── churn_model.joblib
│
├── outputs/
│   └── reports/
│       ├── customer_churn_predictions.csv
│       └── model_metrics.json
│
├── src/
│   ├── config.py
│   ├── data_loader.py
│   ├── preprocessing.py
│   ├── model_training.py
│   └── prediction.py
│
├── app.py
├── main.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <your-repo-link>
cd Customer-Churn-Prediction-Model
```

### 2. Create virtual environment

```bash
python -m venv venv
```

### 3. Activate environment (Windows PowerShell)

```bash
venv\Scripts\Activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

### 🔹 Run Streamlit App

```bash
streamlit run app.py
```

---

### 🔹 Run FastAPI Server

```bash
uvicorn api.fastapi_app:app --reload
```

* API URL: http://127.0.0.1:8000
* Docs: http://127.0.0.1:8000/docs

---

## 🧠 Model Details

* Algorithms Used:

  * Logistic Regression
  * Random Forest

* Preprocessing:

  * Handling missing values
  * Encoding categorical features

* Evaluation Metrics:

  * Accuracy
  * Precision
  * Recall
  * F1-score

---

## 📊 Outputs

* Predictions → `outputs/reports/customer_churn_predictions.csv`
* Metrics → `outputs/reports/model_metrics.json`

---

## 🛠 Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Streamlit
* FastAPI
* Uvicorn
* Matplotlib / Seaborn / Plotly

---

## 🌐 API Example

### POST `/predict`

```json
{
  "tenure": 12,
  "MonthlyCharges": 70.5,
  "Contract": "Month-to-month"
}
```

---

## 👩‍💻 Author

Shrestha Mukherjee

---

## ⭐ Future Improvements

* Deployment (AWS / Render / Railway)
* Authentication system
* Real-time predictions
* Advanced models (XGBoost, Deep Learning)

---

## 📌 Note

Customer churn datasets are usually imbalanced. Proper preprocessing and evaluation are essential for reliable predictions.
