## Project Overview

This project focuses on **long-horizon forecasting of permanent magnet (PM) temperature** in electric motors using a **Long Short-Term Memory (LSTM)** neural network.  
The goal is to accurately predict future thermal behavior based on historical electrical, mechanical, and thermal measurements, which is critical for **thermal safety, efficiency, and predictive control** in electric drive systems.

**Author:** Muhammad Ben Hamad  
**Date:** 2025-12-23  
**Framework:** TensorFlow / Keras  

**Problem Definition:**  
Predict the **PM temperature** at a **future horizon of 80 timesteps (≈ 40 s)** using a **lookback window of 120 timesteps (≈ 60 s)**.  
The task is formulated as a **direct forecasting problem**, where the model outputs a single prediction at the target horizon (no recursive rollout).

**Deployment Target:**  
NEV (New Energy Vehicle) motor temperature monitoring, fault prevention, and predictive thermal control.

---

## Dataset

This project uses the **Electric Motor Temperature Dataset** from Kaggle:

https://www.kaggle.com/datasets/wkirgsn/electric-motor-temperature

The dataset contains synchronized time-series measurements collected from a Permanent Magnet Synchronous Motor (PMSM) under varying operating conditions.

### How to Use the Dataset

1. Download `measures_v2.csv` from Kaggle.
2. Place it in the same directory as the notebook:

```text
pm_lstm_forecast.ipynb
measures_v2.csv
