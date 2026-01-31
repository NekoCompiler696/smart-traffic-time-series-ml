# Smart Traffic Time Series Forecasting

This project focuses on forecasting traffic volume using classical statistical models and deep learning techniques. The objective is to compare traditional time series models with an LSTM-based neural network to evaluate their effectiveness in capturing nonlinear traffic patterns.

---

## 📌 Problem Statement

Accurate traffic forecasting is essential for intelligent transportation systems. Traditional models like ARIMA often struggle with nonlinear and high-frequency data. This project evaluates whether deep learning models, specifically LSTM, provide improved performance over ARIMA and SARIMA.

---

## 📊 Dataset

- Source: Traffic volume dataset
- Frequency: Hourly data
- Target variable: `traffic_volume`

---

## 🧪 Models Implemented

### 1. ARIMA
- Applied on hourly traffic data
- Captures linear temporal dependencies
- Performance degrades on complex patterns

### 2. SARIMA
- Applied on daily aggregated data
- Captures seasonality effectively
- Improved accuracy over ARIMA

### 3. LSTM (Long Short-Term Memory)
- Applied on hourly traffic data
- Captures nonlinear and long-term dependencies
- Best overall performance on high-resolution data

---

## 📈 Evaluation Metrics

| Model | MAE | RMSE |
|------|-----|------|
| ARIMA (Hourly) | 1815.72 | 2062.53 |
| SARIMA (Daily) | 184.33 | 311.58 |
| LSTM (Hourly) | 311.68 | 422.86 |

---

## 📉 Visualization

The project includes visual comparison between actual traffic values and LSTM predictions to validate forecasting performance.

---

## ⚠️ Limitations

- Only traffic volume was used as input; external influencing factors were excluded.
- Limited hyperparameter tuning was performed.
- SARIMA and LSTM were evaluated on different time resolutions.
- No real-time deployment was implemented.

---

## ✅ Conclusion

The LSTM model outperformed ARIMA and demonstrated competitive performance compared to SARIMA while operating on higher-resolution hourly data. This confirms that deep learning approaches are well-suited for complex, nonlinear time series forecasting problems such as traffic prediction.

---

## 🛠 Tools & Technologies

- Python 3.10
- NumPy, Pandas
- Scikit-learn
- TensorFlow / Keras
- Statsmodels
- Matplotlib
