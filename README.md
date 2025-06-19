# Phishing URL Detection using Machine Learning

This project focuses on detecting phishing URLs using supervised machine learning models. It aims to help identify malicious web addresses by extracting key lexical and domain-based features and training classifiers to distinguish between legitimate and phishing URLs.

## 🚀 Demo
You can run the complete project in [Google Colab](https://colab.research.google.com/drive/1zXekO5bfCT2mzhAEU1VM3UnvmY_6yVtJ#scrollTo=QrpPZTukvHZ3).

## 🧠 Project Workflow

### 1. **Data Collection**
- Dataset used: `phishing_site_urls.csv`
- Contains URLs labeled as `phishing` or `legitimate`.

### 2. **Feature Engineering**
- URL-based lexical features are extracted such as:
  - Length of URL
  - Use of `@`, `//`, `-` symbols
  - Presence of IP address in URL
  - Number of subdomains
  - Use of HTTPS
  - Number of digits, special characters, etc.

### 3. **Data Preprocessing**
- Label encoding of the target column.
- Feature scaling using StandardScaler.
- Splitting into training and test sets (70:30 ratio).

### 4. **Model Training**
Implemented and compared the following classifiers:
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- Gradient Boosting
- AdaBoost

### 5. **Evaluation**
- Evaluation metrics used:
  - Accuracy
  - Precision
  - Recall
  - F1-score
- Confusion Matrix and Classification Report generated for each model.
- Random Forest and XGBoost showed the highest accuracy.

### 6. **Prediction**
- Tested model predictions on new sample URLs.
- Pipeline created for feature extraction + model inference.

---

## 🛠️ Tech Stack

| Component        | Technology                        |
|------------------|-----------------------------------|
| Language         | Python 3                          |
| Data Processing  | Pandas, NumPy                     |
| Feature Engineering | Regex, URL parsing modules    |
| Visualization    | Matplotlib, Seaborn               |
| Machine Learning | Scikit-learn, XGBoost             |
| Notebook         | Google Colab                      |

---

## 📁 Repository Structure

```plaintext
phishing_url_detection_ml/
│
├── phishing_url_detection.ipynb   # Main Notebook (Colab-compatible)
├── README.md                      # Project Overview
