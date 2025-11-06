# Demand Forecasting for Electric Vehicle Charging Stations using Multivariate Time Series (2025)

📄 Paper Link: https://arxiv.org/abs/2502.16365  
📂 Local PDF: ../../2502.16365v1.pdf  
✍️ Authors: Zhang et al.  
📌 Publication: arXiv Preprint, 2025  

---

## 🎯 Objective
Develop forecasting models for **EV charging station demand** using **multivariate time series**, integrating:

- Temporal usage patterns
- Weather conditions
- External contextual events

Goal: Improve **resource planning** and **charging infrastructure management**.

---

## 🧠 Key Contributions
- ✅ Incorporates **multiple external features** to improve forecasting accuracy  
  (weather, temperature, public events, etc.)
- ✅ Compares:
  - Classical models (ARIMA, SVR)
  - Deep learning (LSTM, BiLSTM)
- ✅ Highlights importance of correlation among features
- ✅ Shows better performance from **neural networks**

---

## 🧪 Methodology

| Aspect | Description |
|--------|-------------|
| Problem Type | Multivariate forecasting |
| Input Features | Charging demand + exogenous data |
| Target | k-step ahead demand (near horizon) |
| Metrics | MAPE, RMSE |

Forecasting uses different sampling resolutions: hourly / 15-minute intervals.

Data shows:
📌 Weekday vs Weekend behavior = **major demand shift**

---

## 📈 Results
- LSTM outperforms ARIMA and SVR significantly
- Deep models handle **non-linear seasonal patterns**
- Best performance during:
  - Off-peak evening/hours
- Lower performance during:
  - High variation peak periods

⚡ The conclusion realça a necessidade de **modelos mais avançados** para lidar com picos de procura.

---

## ✅ Strengths
- Good real-world context and dataset variety  
- Shows how **external factors** boost predictions  
- Deep learning clearly more reliable than classical models  

---

## ⚠️ Limitations
- Focuses only on **demand load**, not **EV connector availability**
- Prediction limited to **short-term horizons**
- Model interpretability remains low

---

## 📊 Metrics & Results Summary

| Model | RMSE ↓ | MAPE ↓ | MAE ↓ | Observation |
|-------|--------|--------|-------|-------------|
| LSTM | ⭐ Best | ⭐ Best | ⭐ Best | Captures nonlinear + seasonal patterns |
| SVR | Medium | Medium | Medium | Limited handling of dynamic variation |
| ARIMA | Weak | Weak | Weak | Poor performance during high volatility |

Key insights:
- LSTM provides **significant improvements** vs. classical models
- Errors increase during **high-demand peak periods**
- Exogenous features (weather, events) **improve forecasting accuracy**
- Clear weekly and hourly **seasonal patterns**

---

## 🤝 Relevance to CAST Project
✔ Most similar approach to your domain so far ✅  
✔ Motivates using **exogenous features** no teu modelo  
✔ Clear baseline for experimental comparison  
✔ Helps on report section:
**"Forecasting EV charging behavior: literature review"**

---

## 🔍 Tags
EV Charging • Multivariate Time Series • Demand Forecasting • Deep Learning
