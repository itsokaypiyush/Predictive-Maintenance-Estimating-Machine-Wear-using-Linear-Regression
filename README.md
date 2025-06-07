# Predictive-Maintenance-Estimating-Machine-Wear-using-Linear-Regression
# 🚀 Jet Engine Remaining Useful Life Prediction (NASA CMAPSS)

This project predicts the **Remaining Useful Life (RUL)** of turbofan jet engines using supervised learning with **Linear Regression**. It uses the NASA CMAPSS dataset to simulate real-world engine degradation over time.

---

## 📌 Project Highlights

- Dataset: [NASA CMAPSS](https://data.nasa.gov/dataset/Turbofan-engine-degradation-simulation-dataset/ff5v-kuh6)
- Model: Linear Regression
- Evaluation: Manual and library-based MSE, R² Score
- Tooling: Python, Pandas, Scikit-learn, Matplotlib
- Platform: Google Colab

---

## 📁 Dataset Description

Each row in the dataset represents a single cycle of an engine and includes:
- **Engine ID (unit)** and **Cycle number (time)**
- **3 operational settings** (op1, op2, op3)
- **21 sensor measurements** (s1 to s21)
- Target: **Remaining Useful Life (RUL)** — calculated manually

---

## ⚙️ Workflow

1. **Data Preprocessing**
   - Loaded raw `.txt` file and assigned column names
   - Calculated RUL by grouping on engine ID
2. **Feature Selection**
   - Removed non-informative columns (`unit`, `time`)
3. **Model Training**
   - Trained Linear Regression on raw and scaled features
4. **Evaluation**
   - Mean Squared Error (manual + sklearn)
   - R² Score
   - Visualized predictions vs. actual RUL
5. **Improvement**
   - StandardScaler applied for better performance

---

## 📈 Sample Results

| Metric        | Value        |
|---------------|--------------|
| Mean Squared Error | *e.g., 340.21* |
| R² Score           | *e.g., 0.76*   |

> 📊 Visuals included for prediction accuracy and residual analysis

---

## 📦 Requirements

Install via pip or use in Google Colab:

```bash
pip install pandas scikit-learn matplotlib
