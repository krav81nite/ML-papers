# Deep Information Fusion for EV Charging Station Occupancy Forecasting (2021)

📄 Paper Link: https://arxiv.org/abs/2108.12352  
📂 Local PDF: ../../Sao2021.pdf  
✍️ Authors: Sao, Ghimire, Ray  
🏫 Published in: arXiv preprint, 2021  

---

## 🎯 Objective
Predict future **occupancy state** of EV charging stations using **deep learning** with **information fusion** between:

- Temporal charging usage
- Spatial context
- External conditions (e.g., weather)

Output: **Binary classification → Occupied / Free** ✅

---

## 🧠 Key Contributions
- ✅ Combines **static features** (station attributes) + **dynamic temporal data**
- ✅ Introduces deep fusion representation for **spatial-temporal modeling**
- ✅ Improves accuracy vs. classical ML baselines
- ✅ Supports multi-station, multi-connector forecasting

---

## 🧪 Methodology

| Aspect | Description |
|--------|-------------|
| Models | CNN + Dense fusion networks |
| Features | Charging history + location context + temporal metadata |
| Horizon | Short-term occupancy state prediction |
| Data | Real EVSE operational logs |

Incorporates **spatial correlation** between nearby chargers 🤝

---

## 📊 Metrics & Results Summary

| Model | Accuracy ↑ | F1-score ↑ | Observation |
|-------|------------|------------|-------------|
| Deep Fusion Network | ⭐ Best | ⭐ Best | Captures complex spatial-temporal dependencies |
| Classical ML | Medium | Medium | Cannot fuse multi-source information |

Key insights:
- Deep learning **reduces errors** in high-variability environments
- Spatial awareness matters most for **busy urban** charging sites

---

## ✅ Strengths
- Addresses **multi-station** and spatial interdependence
- Better generalization vs single-station ML
- Very close to operational needs of charging networks

---

## ⚠️ Limitations
- Focused on **very short horizon**
- Not optimized for sequential long-term forecasting (like Transformer models)
- Requires richer dataset → sem esses dados, performance cai

---

## 🤝 Relevance to CAST Project
✔ Strong conceptual alignment with **CAST input sources**  
✔ Reinforces benefit of **contextual exogenous features**  
✔ Shows deep learning > classical ML for dynamic EVCS usage  
✔ Great reference in the **Interpretation & Motivation** section

---

## 🔍 Tags
Spatial-Temporal Forecasting • Deep Learning • Availability Prediction • Information Fusion
