# JCDS2804016---Capstone-3_Muhammad-Naufal-Maahir

# 🛍️ E-commerce Customer Churn Classification

Proyek ini merupakan implementasi machine learning untuk memprediksi **customer churn** pada platform e-commerce. Notebook ini dikembangkan sebagai bagian dari **Capstone Project Module 3** (Machine Learning - Classification), sesuai dengan pedoman yang diberikan pada pelatihan Data Science.

---

## 📌 Tujuan Bisnis

Customer churn atau hilangnya pelanggan merupakan salah satu tantangan terbesar dalam industri e-commerce. Tujuan utama proyek ini adalah:

- Memprediksi apakah pelanggan akan **churn (berhenti berlangganan)** berdasarkan data historis.
- Memberikan **insight berbasis data** kepada tim marketing/customer success agar dapat **mengambil tindakan pencegahan**.

---

## 🧠 Problem Statement

Diberikan dataset berisi informasi pelanggan, tugas kita adalah membangun model machine learning untuk memprediksi kolom target `Churn` (0 = tetap, 1 = churn). Model harus:

- Akurat
- Mudah diinterpretasikan
- Siap digunakan dalam produksi

---

## 🧪 Dataset

Dataset yang digunakan bersumber dari file `data_ecommerce_customer_churn.csv` dengan deskripsi fitur berikut:

- `Tenure`, `WarehouseToHome`, `NumberOfDeviceRegistered`, `SatisfactionScore`, dll.
- Fitur kategorikal seperti `PreferedOrderCat`, `MaritalStatus`, `Complaint`
- `Churn` sebagai target label (biner)

📁 Referensi lengkap fitur disediakan di file `E-commerce Customer Churn.docx`.

---

## 🔍 Proses Analisis

1. **Data Cleaning & EDA**  
   - Imputasi missing values  
   - Visualisasi distribusi dan outlier  
   - Korelasi antar fitur

2. **Preprocessing**  
   - Standarisasi numerik, One-Hot Encoding kategorikal  
   - Pipeline dengan `ColumnTransformer`

3. **Modeling**  
   - Model: Random Forest, Gradient Boosting, XGBoost, LightGBM  
   - Hyperparameter tuning via `RandomizedSearchCV`

4. **Ensemble**  
   - Voting dan Stacking (Final model: Stacking dengan Logistic Regression)

5. **Evaluation**  
   - Cross-validation (F1, ROC AUC)  
   - Evaluasi akhir pada test set  
   - Analisis interpretasi menggunakan **SHAP**

---

## 🛠️ Teknologi

- Python (Pandas, Scikit-Learn, XGBoost, LightGBM, SHAP)
- Jupyter Notebook
- Visualisasi: Matplotlib, Seaborn
- Model explainability: SHAP

---
