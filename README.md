# Credit Risk Assessment System

An end-to-end Machine Learning application that predicts the probability of loan default
and categorizes applicants into risk levels using financial and credit-related data.

The system is fully deployed with a FastAPI backend and a Streamlit frontend.

---

## 🚀 Live Demo

**Web Application (Streamlit):**  
👉 https://credit-risk-predictor-15.streamlit.app/

---

## 🧠 Problem Statement

Banks and financial institutions must evaluate the risk associated with loan applicants
before approval. Manual evaluation is slow and subjective.

This system automates credit risk assessment using Machine Learning to support
data-driven lending decisions.

---

## 🎯 Target Users

- Banks & NBFCs (Loan approval support)
- Fintech platforms (Applicant pre-screening)
- Individuals (Credit risk self-assessment)

---

## ⚙️ How the System Works

1. User enters loan and financial details via the web interface
2. Streamlit frontend sends data to FastAPI backend
3. Backend preprocesses inputs using a trained pipeline
4. XGBoost model predicts default probability
5. System returns:
   - Default probability
   - Risk score (0–100)
   - Risk level (Low / Medium / High)
   - Decision recommendation

---

## 🧪 API Example

**POST** `/predict`

```json
{
  "loan_amnt": 250000,
  "term": "36 months",
  "int_rate": 13.5,
  "fico_range_low": 680,
  "annual_inc": 800000,
  "dti": 18.2,
  "emp_length": "5 years",
  "purpose": "debt_consolidation",
  "open_acc": 6,
  "total_acc": 18,
  "revol_util": 45.0,
  "inq_last_6mths": 1
}
```
## 🏗️ System Architecture
Streamlit (Frontend)
        ↓
FastAPI (Backend)
        ↓
Preprocessing Pipeline
        ↓
XGBoost Model

---

## 🛠️ Tech Stack
Python

Pandas, NumPy

Scikit-learn

XGBoost

FastAPI

Streamlit

Deployment:

Render (Backend)

Streamlit Cloud (Frontend)

---

## ☁️ Deployment
Backend deployed using FastAPI on Render

Frontend deployed using Streamlit Community Cloud

Model serialized using a Scikit-learn Pipeline

---

