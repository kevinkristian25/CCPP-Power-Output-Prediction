# CCPP-Power-Output-Prediction
Predicting the hourly net electrical power output (PE) of a Combined Cycle Power Plant (CCPP) using ANN and Random Forest Regressor ($R^2 = 0.9537$). A project for **Engineering Data Science (TF2203**.
---

## 📋 Project Overview
This project aims to predict the net hourly electrical energy output (PE) of a Combined Cycle Power Plant (CCPP) using various Machine Learning architectures. The prediction is based on four environmental input variables:
* **Ambient Temperature (AT)**
* **Ambient Pressure (AP)**
* **Relative Humidity (RH)**
* **Exhaust Vacuum (V)**

The dataset consists of **9,568 hourly measurements** collected from the UCI Machine Learning Repository.

## ⚙️ Methodology
I developed and compared four different model architectures to identify the most effective approach for this thermodynamic dataset:
1. **Baseline Models:** Artificial Neural Network (ANN) and Random Forest Regressor.
2. **Sequential Models:** Long Short-Term Memory (LSTM) and Gated Recurrent Unit (GRU) to explore potential temporal patterns.

## 🚀 Key Results
Through extensive hyperparameter tuning and cross-validation, the **Random Forest** model emerged as the superior solution:
* **R-Squared ($R^2$):** **0.9537** (explaining 95% of data variability).
* **RMSE:** **3.6259 MW**.
* **Efficiency:** Achieved the fastest prediction time of **0.0170 seconds**, making it ideal for low-latency industrial applications.

## 💡 Conclusion
The analysis proves that tabular regression models (Random Forest and ANN) significantly outperform sequential deep learning models (LSTM and GRU) for this specific CCPP dataset. This is because the relationship between the environmental variables and power output occurs instantaneously rather than through long-term temporal dependencies.

## 📂 Files in this Repository
* `Metode_Acuan_dengan_Random_Forest.ipynb`: Implementation and optimization of the best-performing model.
* `Metode_Acuan_dengan_MLP_sederhana_(ANN).ipynb`: Baseline Neural Network implementation.
* `Metode_Kembangan_LSTM&GRU.ipynb`: Exploration of recurrent architectures.
* `LAPORAN TUGAS BESAR-211.pdf`: Full technical report in Indonesian.
