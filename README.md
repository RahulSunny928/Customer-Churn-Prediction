# 📊 Customer Churn Prediction

This project predicts **customer churn** using the **Telco Customer Churn dataset**.  
It applies data preprocessing, feature engineering, and advanced ensemble machine learning techniques to identify customers who are most likely to leave a telecom service provider.

---

## 🚀 Project Description

**Objective:**  
Predict whether a customer will churn based on their demographic, contract, and service-related details.

**Dataset:**  
`Telco-Customer-Churn-dataset-cleaned.csv` (included in this repository)

**Approach:**
1. Exploratory Data Analysis (EDA)  
2. Feature engineering & encoding  
3. Model training using **XGBoost**, **LightGBM**, and **CatBoost**  
4. Hyperparameter tuning with **Optuna**  
5. Ensemble stacking for improved performance  

**Result:**  
Final model achieves approximately **0.85 AUC score** on the test set.

---

## 🛠️ Tech Stack & Libraries

**Language:** Python 3.x  

**Core Libraries:**
- scikit-learn  
- xgboost  
- lightgbm  
- catboost  
- optuna  
- numpy, pandas  
- matplotlib, seaborn, plotly  

---

## 📂 Project Structure



Customer-Churn-Prediction/
│── Telco-Customer-Churn-dataset-cleaned.csv # Cleaned dataset
│── Telco-Customer-Churn-Prediction.ipynb # Main Jupyter Notebook
│── Telco-Customer-Churn-Prediction.html # Notebook HTML export
│── XGB_Hyperparameter.pickle # Saved XGBoost best params
│── LGBM_Hyperparameter.pickle # Saved LightGBM best params
│── CatBoost_Hyperparameter.pickle # Saved CatBoost best params
│── model_catboost/ # Trained CatBoost model files
│── catboost_info/ # CatBoost logs/info
│── requirements.txt # Dependencies
│── README.md # Project documentation


---

## ⚙️ Requirements

Make sure you have **Python 3.x** installed.  
Then, install the required libraries:

```bash
pip install -r requirements.txt

🗄️ Database / Data Setup

No external database required.

Data is already provided in CSV format:
Telco-Customer-Churn-dataset-cleaned.csv

(Optional) You can import the CSV into a database (MySQL/PostgreSQL) and modify the notebook to fetch from there.

▶️ How to Run Locally
1️⃣ Clone the Repository
git clone https://github.com/vishred06-cmd/Customer-Churn-Prediction.git
cd Customer-Churn-Prediction

2️⃣ Create a Virtual Environment (recommended)
python -m venv venv


Activate it:

Windows:

venv\Scripts\activate


Mac/Linux:

source venv/bin/activate

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Run the Jupyter Notebook
jupyter notebook Telco-Customer-Churn-Prediction.ipynb


👉 Alternatively, open the pre-rendered HTML report:
Telco-Customer-Churn-Prediction.html in your browser to view results directly.

5️⃣ Using Saved Models / Hyperparameters

Pre-tuned hyperparameters (.pickle files) are available for direct use.

The CatBoost model inside model_catboost/ can be loaded for predictions.

📜 License

This project is licensed under the MIT License.
You are free to use, modify, and distribute it with attribution.

🙌 Acknowledgements

Dataset: IBM Telco Customer Churn Dataset (available on Kaggle)

Thanks to the open-source contributors of:

Scikit-learn

XGBoost

LightGBM

CatBoost

Optuna
