# CCPP-Power-Output-Prediction
Predicting the hourly net electrical power output (PE) of a Combined Cycle Power Plant (CCPP) using ANN and Random Forest Regressor ($R^2 = 0.9537$). A project for Engineering Data Science (TF2203).
# Electrical Power Output Prediction for CCPP

Predicting the hourly net electrical power output (PE) of a Combined Cycle Power Plant (CCPP) using ANN and Random Forest Regressor ($R^2 = 0.9537$). A project for **Engineering Data Science (TF2203)**.

---

## 📋 Project Overview
This project aims to predict the net hourly electrical energy output (PE) of a Combined Cycle Power Plant (CCPP) using various Machine Learning architectures. The prediction is based on four environmental input variables:
* **Ambient Temperature (AT)**
* **Ambient Pressure (AP)**
* **Relative Humidity (RH)**
* **Exhaust Vacuum (V)**

[cite_start]The dataset consists of **9,568 hourly measurements** collected from the UCI Machine Learning Repository[cite: 112, 114].

## ⚙️ Methodology
I developed and compared four different model architectures to identify the most effective approach for this thermodynamic dataset [cite: 109, 123-126]:
1. **Baseline Models:** Artificial Neural Network (ANN) and Random Forest Regressor[cite: 110].
2. **Sequential Models:** Long Short-Term Memory (LSTM) and Gated Recurrent Unit (GRU) to explore potential temporal patterns[cite: 111].

## 🚀 Key Results
Through extensive hyperparameter tuning and cross-validation, the **Random Forest** model emerged as the superior solution[cite: 272, 273, 335]:
* **R-Squared ($R^2$):** **0.9537** (explaining 95% of data variability)[cite: 337].
* **RMSE:** **3.6259 MW**[cite: 338].
* **Efficiency:** Achieved the fastest prediction time of **0.0170 seconds**, making it ideal for low-latency industrial applications[cite: 352, 383].

## 💡 Conclusion
[cite_start]The analysis proves that tabular regression models (Random Forest and ANN) significantly outperform sequential deep learning models (LSTM and GRU) for this specific CCPP dataset [cite: 387-393]. [cite_start]This is because the relationship between the environmental variables and power output occurs instantaneously rather than through long-term temporal dependencies[cite: 397].

## 📂 Files in this Repository
* `Metode_Acuan_dengan_Random_Forest.ipynb`: Implementation and optimization of the best-performing model [cite: 134-137].
* `Metode_Acuan_dengan_MLP_sederhana_(ANN).ipynb`: Baseline Neural Network implementation [cite: 161-163].
* `Metode_Kembangan_LSTM&GRU.ipynb`: Exploration of recurrent architectures [cite: 174-188].
* `LAPORAN TUGAS BESAR-211.pdf`: Full technical report in Indonesian[cite: 84].
