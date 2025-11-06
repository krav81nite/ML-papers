# Forecasting Charging Point Occupancy Using Supervised Learning Algorithms (2022)

📄 Paper Link: https://www.mdpi.com/1996-1073/15/9/3409  
📂 Local PDF: ../../Ostermann2022.pdf  
✍️ Authors: Ostermann, Kahlen & van Dinther  
🏫 Published in: Energies (MDPI), 2022  

---

## 🎯 Objective
Predict **charging point occupancy** status using **supervised learning classifiers**  
Output: **Binary state → Occupied (1) / Free (0)**

Goal: Help operators improve **resource management** by anticipating charging demand.

---

## 🧠 Key Contributions
- ✅ First **comparative** ML study specifically on EV **occupancy state**
- ✅ Focus on classification instead of load forecasting
- ✅ Includes **dynamic and contextual** features (e.g., time, traffic)
- ✅ Uses station-level individual connectors, not aggregated demand

---

## 🧪 Methodology

| Aspect | Description |
|--------|-------------|
| Input Features | Timestamp, day-of-week, type of charger, station location |
| Horizons | Up to 30 minutes ahead |
| Models Tested | Logistic Regression, Random Forest, XGBoost |
| Dataset | Public charging infrastructure datasets |

---

## 📊 Metrics & Results Summary

| Model | Accuracy ↑ | Precision ↑ | Recall ↑ | Observation |
|-------|------------|-------------|----------|------------|
| XGBoost | ⭐ Best | ⭐ Best | ⭐ Best | Captures complex usage patterns |
| Random Forest | High | High | Medium | Robust with lower variance |
| Logistic Regression | Medium | Medium | Medium | Struggles with nonlinear effects |

Key findings:
- Accuracy declines **non-linearly** with horizon length
- **Seasonality (weekday vs weekend)** strongly affects usage
- Extreme peaks remain hard to predict

---

## ✅ Strengths
- Very aligned with **predicting charger availability**
- Points out key operational challenges (rush hours, events)
- Clear metrics → useful for comparison benchmarks

---

## ⚠️ Limitations
- Short-term only (under 30 min)
- Classical ML performance plateaus quickly
- No time-series deep learning baselines included

---

## 🤝 Relevance to CAST Project
✔ Same problem as CAST → **Station availability classification**  
✔ Baselines to compare **CAST (DL)** vs **classical ML**  
✔ Highlights contextual features → importante para abalar desempenho  
✔ Excelente suporte à tua motivação no relatório ✅

---

## 🔍
