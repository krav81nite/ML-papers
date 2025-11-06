# Charging Stations Demand Forecasting using LSTM-Based Hybrid Transformer Model (2025)

📄 Paper Link: https://doi.org/10.1038/s41598-025-20421-y  
📂 Local PDF: ../../s41598-025-20421-y.pdf  
✍️ Authors: Kanters et al.  
🏫 Published in: Scientific Reports (Nature Portfolio), 2025  

---

## 🎯 Objective
Propose a **hybrid LSTM-Transformer model** to improve EV charging **demand forecasting** accuracy by learning:

- Short-term temporal dependencies (via LSTM)
- Long-term relationships and attention patterns (via Transformer)

Target use case:
📌 Help decision-making for **charging infrastructure planning**

---

## 🧠 Key Contributions
- ✅ Novel **hybrid architecture** combining strengths of:
  - LSTM → local temporal memory
  - Transformer → global attention for long sequences
- ✅ Demonstrates real-world performance on EV charging datasets
- ✅ Shows attention improves modeling of **spatial-temporal dependencies**
- ✅ Offers a balance between **accuracy** and **computational cost**

---

## 🧪 Methodology

| Component | Role |
|----------|------|
| LSTM layers | Extract near-term dynamics |
| Transformer encoder | Capture long-range dependencies |
| Fusion layer | Combine representations |
| Dense head | Multi-step forecasting output |

Metrics:
- MAE
- RMSE
- MAPE

Comparison models:
- Standalone LSTM
- ARIMA
- Random Forest

---

## 📈 Results

| Model | Performance |
|-------|-------------|
| Hybrid Transformer-LSTM | ⭐ Best |
| LSTM only | Good but weaker long-term |
| ARIMA | Struggles at peak hours |

Insights:
- More connectors → higher variance → harder peaks
- Spatial location strongly influences demand

🧠 High take-away:
➡️ Pure deep learning already **beats classical models**  
➡️ Adding attention **further improves forecast quality**

---

## ✅ Strengths
- Very aligned with **spatio-temporal forecasting**
- Well-balanced architecture complexity
- Highly relevant to real EV infrastructure systems

---

## ⚠️ Limitations
- Focuses only on **load** — does not yet model **availability state**
- Dataset not public → reproducibility limitada
- Interpretability limitada vs TFT approach

---

## 📊 Metrics & Results Summary

| Model | RMSE ↓ | MAPE ↓ | MAE ↓ | Observation |
|-------|--------|--------|-------|-------------|
| Hybrid Transformer–LSTM | ⭐ Best | ⭐ Best | ⭐ Best | Captures long-range + local dynamics; most robust at multi-step horizons |
| LSTM (standalone) | Medium | Medium | Medium | Good short-term memory; weaker for long seasonal effects |
| ARIMA / Classical | Weak | Weak | Weak | Struggles during peak hours and regime shifts |

Key insights:
- Attention layers **improve long-horizon accuracy** over LSTM-only
- Performance degrades slightly in **high-variance peak periods**, but still superior to baselines
- Spatial/context features materially **boost** results (e.g., station/location effects)

---

## 🤝 Relevance to CAST Project
⭐⭐⭐ ALTAMENTE RELEVANTE ⭐⭐⭐

✔ Justifica:
- Hybrid models (RNN + Transformer)
- Attention for EV charging
- Focus on real operational use cases

✔ Ajudará muito na tua **Introdução + Estado da Arte**  
✔ Excelente referência para comparar resultados do CAST

---

## 🔍 Tags
EV Charging • Hybrid Model • Transformer • LSTM • Demand Forecasting
