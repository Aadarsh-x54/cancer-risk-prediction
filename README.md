# Cancer Risk Level Prediction

An end-to-end Machine Learning web application built using **Streamlit**, **Scikit-Learn**, and **XGBoost** to assess cancer risk levels (Low, Medium, High) based on clinical and lifestyle risk factors.

---

## Overview

This project provides an interactive tool for predicting cancer risk using an optimized class-weighted XGBoost classifier. Users can submit single patient records via an intuitive interactive form or upload CSV files for batch predictions with probability breakdowns.

---

## Features

- **Interactive Web UI**: Built with Streamlit for seamless user experience.
- **Batch Evaluation**: Upload CSV files containing patient data to generate batch predictions and download the output.
- **Single Patient Risk Assessment**: Input individual feature values through interactive controls to receive instant predictions with class confidence scores.
- **Probability Breakdown**: Displays predicted risk levels accompanied by probability scores for Low, Medium, and High risk categories.

---

## Project Structure

```text
├── app.py                            # Streamlit frontend & inference pipeline
├── Cancer_Risk_Prediction_(ML).ipynb # Model training & evaluation notebook
├── cancer-risk-factors.csv           # Dataset used for training and testing
├── final_xgb_class_weighted.pkl      # Serialized XGBoost model
├── label_encoder.pkl                 # Target label encoder
├── feature_names.pkl                 # Ordered list of feature columns
├── requirements.txt                  # Python dependencies
└── README.md                         # Documentation
```

---

## Getting Started

### 1. Prerequisites
- Python 3.10+
- `pip` package manager

### 2. Setup Virtual Environment

**Windows:**
```powershell
python -m venv .venv
.venv\Scripts\activate
```

**Linux / macOS:**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
streamlit run app.py
```

Open your browser and navigate to `http://localhost:8501`.
