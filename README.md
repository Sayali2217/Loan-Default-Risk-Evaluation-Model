Here is a **clean, well-formatted, GitHub-ready README.md** version of your content—proper headings, spacing, lists, and structure.

---

# **CreditIQ – Loan Default Risk Evaluation**

CreditIQ is a **Machine Learning–based risk intelligence platform** designed to predict loan default probability using structured financial data and document-derived insights.
The system combines **predictive modeling**, **explainable AI**, and **document processing** to support **data-driven credit decisions**.

---

##  **Problem Statement**

Traditional credit evaluation systems suffer from:

*  Inaccurate risk assessment
*  Lack of interpretability
*  Inefficient manual document verification
*  Delayed decision-making

**CreditIQ** addresses these limitations by building an **automated, explainable, and scalable credit risk assessment system**.

---

## ⚙️ **Machine Learning Approach**

### **1. Data Processing**

* Feature engineering on financial & behavioral attributes
* Handling missing values
* Categorical encoding
* Feature scaling using standardization

### **2. Model Selection**

* **LightGBM (Gradient Boosting)**
* Optimized for **tabular data**, large datasets, and complex feature interactions

### **3. Training Details**

* **Dataset size:** ~8,000 loan records
* **Features:** 40+ engineered features
* **Target:** Binary classification (Loan Default: 0/1)

### **4. Evaluation Metrics**

| Metric       | Score |
| ------------ | ----- |
| **AUC-ROC**  | ~0.90 |
| **AUC-PR**   | ~0.81 |
| **F1 Score** | ~0.73 |

These metrics demonstrate **strong predictive performance** and **balanced precision–recall** behavior.

---

## 🔍 **Explainability (Model Interpretability)**

To reduce the "black-box" nature of ML models:

* Implemented **SHAP (SHapley Additive exPlanations)**
* Provides **feature-level contributions** for each prediction
* Improves **transparency** and **trust** in financial decisions
* Essential for compliance-driven credit risk evaluation

---

## 🏗️ **System Architecture**

1. User inputs financial details **or uploads documents**
2. **OCR** extracts relevant text (Tesseract)
3. Data undergoes **processing & feature transformation**
4. **ML model** predicts default probability
5. **SHAP** generates explanations
6. Interactive results displayed on **Streamlit dashboard**

---

## 📄 **OCR Integration**

* Powered by **Tesseract OCR**
* Extracts structured data from bank statements / financial documents
* Minimizes manual entry and increases processing speed

---

## 🛠️ **Tech Stack**

| Layer              | Technologies           |
| ------------------ | ---------------------- |
| **Frontend**       | Streamlit              |
| **Backend**        | Python                 |
| **ML**             | LightGBM, Scikit-learn |
| **Explainability** | SHAP                   |
| **OCR**            | Tesseract              |
| **Visualization**  | Plotly, Matplotlib     |

---

## 📂 **Project Structure**

```
loan-risk-app/
│── app.py
│── loan_pipeline.pkl
│── scaler.pkl
│── feature_cols.json
│── threshold.txt
│── requirements.txt
│── .env (ignored)
│── .gitignore
│── assets/
```

---

## 🚀 **Installation & Setup**

### **1. Clone the repository**

```bash
git clone https://github.com/Kalyanie139/loan-defaut-risk-evaluation.git
cd loan-risk-app
```

### **2. Create virtual environment**

```bash
python -m venv venv
source venv/bin/activate
```

### **3. Install dependencies**

```bash
pip install -r requirements.txt
```

### **4. Add environment variables**

Create a `.env` file:

```
API_KEY=your_api_key_here
```

### **5. Run the application**

```bash
streamlit run app.py
```

---

## 🌟 **Key Features**

* Real-time **loan default prediction**
* **Explainable AI** with SHAP feature attributions
* **Document-based data extraction** via OCR
* Interactive **visualization dashboard**
* Fully **modular**, easy to scale and integrate

---

## 💼 **Use Cases**

* Banking & Financial Institutions
* Credit Risk Assessment Platforms
* FinTech Loan Approval Systems
* Automated Underwriting Pipelines

---

## 📈 **Future Improvements**

* Integration of **RBI guideline-based rule engine**
* Automated **model retraining & monitoring**
* Cloud deployment (AWS/GCP/Azure)
* Enhanced feature engineering with external bureau data

---

## 👩‍💻 **Author**

**Sayali Shirode**
GitHub: [https://github.com/Sayali2217](https://github.com/Sayali2217)

---

## 📜 **License**

This project is for **educational and demonstration purposes**.

