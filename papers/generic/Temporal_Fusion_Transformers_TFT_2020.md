# Temporal Fusion Transformers for Interpretable Multi-Horizon Time Series Forecasting (2020)

📄 Paper Link: https://arxiv.org/abs/1912.09363  
📂 Local PDF: ../../1912.09363v3.pdf  
✍️ Authors: Lim et al.  
🏫 Published in: NeurIPS 2020  

---

## 🎯 Objective
Propose a new Transformer-based architecture that effectively models **complex time series with multiple inputs** and provides **interpretability** through attention mechanisms and variable selection.

---

## 🧠 Key Contributions
- ✅ Introduces **Variable Selection Networks** for handling many features
- ✅ Integrates **static, known future, and historical inputs** effectively
- ✅ Provides **interpretability** via attention weights
- ✅ Achieves **state-of-the-art forecasting performance** on several datasets
- ✅ Designed specifically for **forecasting** (not NLP)

---

## 🧪 Methodology
| Component | Purpose |
|----------|---------|
| LSTM Encoder | Learn temporal dynamics |
| Multi-Head Attention | Focus on relevant temporal patterns |
| Gating Mechanisms | Improve stability and prevent overfitting |
| Variable Selection | Identify most important features |

📌 Forecasting type: **multi-horizon**  
(ex.: next 24 steps)

Loss: Quantile loss → supports **probabilistic forecasting**

---

## 📈 Results
- Outperforms models like:
  - DeepAR
  - LSTM
  - Seq2Seq
- Gains are strongest when **many features** influence the target

Interpretability examples:
- Feature importance scores
- Temporal attention heatmaps

---

## ✅ Strengths
- Designed for **real-world forecasting tasks**
- Handles **external/contextual variables** (calendar, location…)
- Built-in **explainability**, helping decision-makers
- Better generalization with gating layers

---

## ⚠️ Limitations
- More complex to train than basic Transformers/LSTMs
- Still suffers from **quadratic attention** complexity
- Interpretability can add computational overhead

---

## 🤝 Relevance to CAST Project
✔ Allows incorporation of **EV station metadata**  
✔ Shows which variables matter most:
- 🚗 usage patterns
- 🕒 time of day / weekday
- 📍 geolocation  
✔ Useful for **availability prediction** at different horizons  
✔ Good candidate to compare against Informer and basic Transformer

---

## 🔍 Tags
Time Series • Transformers • Forecasting • Interpretability • EV Charging
