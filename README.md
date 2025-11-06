# ML-papers
# 📚 Research Paper Repository — CAST Project

This repository collects and organizes scientific papers that support the CAST
(Charging Availability Sequence Transformer) research project.  
Papers are organized into two core categories:

- ✅ Generic Papers → Technical foundations (Deep Learning for sequence modeling)
- ✅ Focused Papers → Applications to EV charging forecasting

A progress tracker is also included for each paper.

---

## 🔹 Generic Papers (Technical Foundations)

| Paper | Topic | Status |
|-------|-------|:-----:|
| [Attention Is All You Need (2017)](papers/generic/Attention_Is_All_You_Need_2017.md) | Transformer Encoder-Decoder | ⬜ |
| [Temporal Fusion Transformers (2020)](papers/generic/Temporal_Fusion_Transformers_TFT_2020.md) | Context-aware forecasting | ⬜ |
| [Balanced Frequency Adaptive Tuning — BEAT (2025)](papers/generic/Balanced_Frequency_Adaptive_Tuning_BEAT_2025.md) | Long-term TS forecasting | ⬜ |
| [Sequence-to-Sequence Learning (2014)](papers/generic/Sequence_to_Sequence_Learning_Sutskever2014.md) | Seq2Seq architecture | ⬜ |
| [Long Short-Term Memory (1997)](papers/generic/Long_Short_Term_Memory_1997.md) | RNN variant for long memory | ⬜ |
| [Informer (2020)](papers/generic/Informer_Long_Sequence_TimeSeries_Forecasting_2020.md) | Efficient TS Transformer | ⬜ |

---

## 🔹 Focused Papers (EV Charging Forecasting)

| Paper | Topic | Status |
|-------|-------|:-----:|
| [Time-Series Modeling of Aggregated EV Charging Load (2017)](papers/focused/TimeSeries_Modeling_Aggregated_EV_Charging_Load_Louie2017.md) | EV charging load modeling | ⬜ |
| [Demand Forecasting for EV Charging Stations using Multivariate TS (2025)](papers/focused/Demand_Forecasting_EV_Charging_Stations_MultivariateTS_2025.md) | Multivariate TS for charging demand | ⬜ |
| [EV Charging Station Demand Forecasting using LSTM-Based Hybrid Transformer (2025)](papers/focused/Charging_Stations_Demand_Forecasting_LSTM_Hybrid_Transformer_2025.md) | Hybrid model for station demand | ⬜ |

---

📌 **Legend for Status column**  
⬜ Not started | 🔄 Reading / notes in progress | ✅ Completed

---

> ✨ When writing the final report, this structure allows quick reference
> for the State-of-the-Art chapter and citations.

---

---

## 📚 Bibliography Management

All scientific references for this repository are maintained in:

📌 [`bibliography.bib`](papers/bibliography.bib)

---

## 📊 Focused Papers — Comparative Summary

| Paper | Forecast Target | Dataset Type | ML Approach | Best Model | Metrics | Horizon | Key Challenge | Relevance to CAST |
|-------|----------------|--------------|-------------|------------|---------|---------|----------------|------------------|
| Louie et al. (2017) | Aggregated Load | Real-world EVCS | Classical TS | ARIMA (off-peak) | RMSE, MAPE | Short | High peak variance | Motivates deep methods |
| Zhang et al. (2025) | Load (multivariate) | Real EVCS + Weather | DL (LSTM) | LSTM | RMSE, MAPE, MAE | Short | Nonlinear seasonal effects | Supports exogenous features |
| Kanters et al. (2025) | Demand (station) | Multi-station | Hybrid (LSTM+Transformer) | Hybrid | RMSE, MAPE, MAE | Short-Mid | Long-term patterns | Attention improves results |
| Soldan et al. (2021) | Occupancy (binary) | Real EVCS logs | ML (Streaming) | RF | Accuracy, F1 | 5–30 min | Horizon worsens classifiers | Baseline for CAST classifier |
| Ostermann et al. (2022) | Charging point status | Public charging infra | Classical ML | XGBoost | Accuracy, Precision, Recall | <30 min | Daily cycles | Feature engineering matters |
| Sao et al. (2021) | Occupancy (binary) | Spatial-temporal | DL (Fusion) | Deep Fusion CNN | Accuracy, F1 | Short | Spatial dynamics | Multi-station modeling justified |
| Douaidi et al. (2025) | Occupancy (binary) | Multi-operator | Federated DL | FedAvg Hybrid | Accuracy, Precision, Recall | Short | Privacy + heterogeneity | Future CAST deployment scenario |


---

### ✅ Main Conclusions

The reviewed literature on forecasting in EV charging infrastructure reveals three clear stages of evolution:

1️⃣ **Classical time-series and ML methods**  
(e.g., ARIMA, Logistic Regression, Random Forest)  
→ Perform reasonably well during predictable periods, but struggle with peak-time volatility and long-horizon behavior.

2️⃣ **Deep learning-based forecasting**  
(e.g., LSTM, CNN fusion)  
→ Superior for nonlinear and spatial-temporal EV usage patterns, especially in urban and multi-station contexts.

3️⃣ **Deployment-aware architectures**  
(e.g., Federated Deep Learning)  
→ Address privacy, heterogeneous data sources, and real-world multi-operator constraints.

---

#### ✅ Gap identified in the state-of-the-art

While some papers perform **binary occupancy forecasting** (Occupied vs Free), existing models:

- ❌ Rarely model **sequential temporal dependency** across multiple future steps  
- ❌ Provide limited interpretability for operational decision-making  
- ❌ Lack unified modeling across **multiple stations** and horizons  
- ❌ Focus primarily on **short-term** (< 30 min) forecasts  

---

### 🚀 CAST — Charging Availability Sequence Transformer

To address these gaps, **CAST** aims to:

✅ Predict **charging availability state** (binary/multiclass)  
✅ Across **multiple horizons** (short to mid-term)  
✅ Using **advanced sequential modeling** (Transformers)  
✅ Allow inclusion of **contextual features** (temporal, spatial, operational)  

📌 This positions CAST as a **novel and relevant** contribution to forecasting in EV charging infrastructure.







