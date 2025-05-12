
# 🧠 Customer Churn Prediction App

This is a **Streamlit web application** that predicts whether a customer is likely to churn based on their profile information such as geography, gender, credit score, balance, and more.

🔗 **Live App**: [Click here to try it out!](https://churn-prediction-ann-cls.streamlit.app/)

## 🚀 Features

- 📊 User-friendly interface to input customer data
- 🔍 Real-time prediction of churn probability
- 📈 Model trained using TensorFlow on a bank customer dataset
- 🔄 Uses `LabelEncoder`, `OneHotEncoder`, and `StandardScaler` for preprocessing
- ✅ Deployable with Streamlit Cloud or locally

## 🧩 Input Features

The app takes the following inputs from the user:

- **Geography**: Country of residence (one-hot encoded)
- **Gender**: Male or Female (label encoded)
- **Age**
- **Credit Score**
- **Tenure**: Years of relationship with the bank
- **Balance**
- **Number of Products**: Bank products owned by the customer
- **Has Credit Card**: Whether the customer has a credit card (0 or 1)
- **Is Active Member**: Whether the customer is an active member (0 or 1)
- **Estimated Salary**

## 🛠️ Tech Stack

- **Frontend**: Streamlit
- **Model**: TensorFlow / Keras
- **Preprocessing**: Scikit-learn (`LabelEncoder`, `OneHotEncoder`, `StandardScaler`)
- **Language**: Python


## ▶️ How to Run the App Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/churn-prediction-app.git
   cd churn-prediction-app
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## 📈 Model Training (Optional)

If you want to retrain the model:
- Use a dataset like `Churn_Modelling.csv`
- Preprocess categorical and numerical features
- Train a binary classifier using TensorFlow/Keras
- Save the model and encoders using `pickle`

## 🧪 Sample Dataset Format

Example row from training dataset (`Churn_Modelling.csv`):

```
RowNumber,CustomerId,Surname,CreditScore,Geography,Gender,Age,Tenure,Balance,NumOfProducts,HasCrCard,IsActiveMember,EstimatedSalary,Exited
```

## 📜 License

This project is licensed under the MIT License.
