# Short-Term Forecast of EV Charging Stations Occupancy Probability Using Big Data Streaming Analysis (2021)

📄 Paper Link: https://arxiv.org/pdf/2104.12503  
📂 Local PDF: ../../Soldan2021.pdf  
✍️ Authors: Soldan, Macek & Petru  
🏫 Published in: IEEE Transactions — Big Data Applications (2021)  

---

## 🎯 Objective
Forecast occupancy of EV charging stations in the **next 5–30 minutes** using **streaming-based** machine learning models.

Task: **Binary classification**  
→ *Occupied (1) vs. Free (0)*

---

## 🧠 Key Contributions
- ✅ Real-time occupancy prediction from **live streaming EVSE data**
- ✅ Binary classification formulation
- ✅ Demonstrates feasibility of fast decision support systems
- ✅ Uses scalable big data pipelines

---

## 🧪 Methodology

| Aspect | Description |
|--------|-------------|
| Input | Timestamped transactions + connector status |
| Prediction Horizon | 5–30 minutes ahead |
| Models | Logistic Regression, Random Forest |
| Deployment | Streaming environment (Spark Structured Streaming) |

---

## 📊 Metrics & Results Summary

| Model | Accuracy ↑ | F1-score ↑ | Observation |
|-------|------------|------------|------------|
| Random Forest | ⭐ Best | ⭐ Best | Captures nonlinearity in behavior |
| Logistic Regression | Good | Medium | Faster inference; lower peaks performance |

Key findings:
- Even simple ML → viable for occupancy state classification
- Accuracy decreases with **longer horizons**

---

## ✅ Strengths
- Efficient for real-time operational use cases
- Low computational overhead
- First practical demonstration of occupancy prediction pipeline

---

## ⚠️ Limitations
- Feature set limited (misses weather, holidays…)
- Short-term forecast only
- No deep learning → limited long-range pattern modeling

---

## 🤝 Relevance to CAST Project
✔ Same prediction target: **Occupied vs Free**  
✔ Strong motivation for real-time availability forecasting  
✔ Can be a baseline vs. your Transformer model  
✔ Supports architectural decision: deep learning → better horizons

---

## 🔍 Tags
Binary Classification • Streaming Analytics • EV Charging Availability • Machine Learning
