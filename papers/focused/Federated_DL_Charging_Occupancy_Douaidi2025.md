# Federated Deep Learning for Enhanced Prediction of Charging Station Occupancy (2025)

📄 Paper Link: https://opeva.eu/wp-content/uploads/2025/02/Journal___Charging_station_occupancy_prediction.pdf  
📂 Local PDF: ../../Douaidi2025.pdf  
✍️ Authors: Douaidi, Lugaresi, Verzola, Gross et al.  
🏫 Published in: Journal under review — OPEVA project, 2025  

---

## 🎯 Objective
Predict **binary occupancy state** of EV charging stations using a **federated deep learning architecture** that:

- Preserves **data privacy**
- Improves **generalization** across multiple station networks
- Supports **real-world distributed forecasting**

---

## 🧠 Key Contributions
- ✅ First approach using **Federated Learning** in EV availability prediction  
- ✅ Hybrid CNN–LSTM model used in local nodes  
- ✅ Global model updated without sharing sensitive usage data  
- ✅ Shows stability in heterogeneous charging networks

---

## 🧪 Methodology

| Aspect | Description |
|--------|-------------|
| Learning Approach | Federated averaging (FedAvg) |
| Local Models | CNN + LSTM fusion |
| Output | Occupied / Free |
| Benchmarks | Centralized DL, Local-only training |
| Dataset | Multi-provider EVCS datasets |

Federated approach **reduces privacy risks** and **distribution shift issues** ✅

---

## 📊 Metrics & Results Summary

| Model | Accuracy ↑ | Precision ↑ | Recall ↑ | Observation |
|-------|------------|-------------|----------|------------|
| Federated DL (FedAvg) | ⭐ Best | ⭐ Best | ⭐ Best | Handles multiple regions and operator heterogeneity |
| Centralized DL | Medium | Medium | Medium | Sensitive to domain shift |
| Local-only DL | Lower | Lower | Lower | Overfits to local patterns |

Key Insights:
- Federated learning improves prediction in **new/unseen stations**
- Communication efficiency remains a challenge

---

## ✅ Strengths
- Directly aligned with **privacy constraints in EV networks**
- Highly scalable for **nationwide** charging infrastructure
- Supports **multi-station** and **multi-operator** forecasting

---

## ⚠️ Limitations
- Communication overhead between nodes
- Complex deployment requirements
- Still emerging research — not widely validated

---

## 🤝 Relevance to CAST Project
✔ Demonstrates advanced **deployment-aware** approaches  
✔ Useful for future work section: CAST could incorporate federated training  
✔ Supports multi-operator scaling without sharing private data  
✔ Bridges gap between ML development & real-world infrastructure

---

## 🔍 Tags
Federated Learning • EV Availability • CNN-LSTM • Privacy-Preserving ML
