# 📈 Anomaly Detection in Time Series using Autoencoders

This project trains a deep **LSTM Autoencoder** to detect anomalies in sensor data based on reconstruction error.

---

## 🧪 Dataset Format

CSV file `sensor.csv` should look like:

| timestamp         | value  |
|------------------|--------|
| 2023-01-01 00:00 | 0.13   |
| 2023-01-01 00:01 | 0.11   |

---

## Model

- **Encoder**: LSTM (64 units)
- **Decoder**: LSTM + TimeDistributed
- **Loss**: Mean Squared Error (MSE)
- **Anomaly threshold**: 95th percentile of train loss

---

## 🚀 Run This Project

Install dependencies:

```bash
pip install tensorflow pandas matplotlib scikit-learn
