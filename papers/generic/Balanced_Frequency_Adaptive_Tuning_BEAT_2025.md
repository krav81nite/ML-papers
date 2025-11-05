# BEAT: Balanced Frequency Adaptive Tuning for Long-Term Time-Series Forecasting (2025)

📄 Paper Link: https://arxiv.org/abs/2501.19065  
📂 Local PDF: ../../2501.19065v2.pdf  
✍️ Authors: Xu et al.  
📌 Publication: Under review / arXiv preprint (2025)  

---

## 🎯 Objective
Improve long-term time series forecasting by addressing frequency bias issues present in current Transformer-based models, enabling better stability and generalization over extended horizons.

---

## 🧠 Key Contributions
- ✅ Introduces **Balanced Frequency Adaptation (BFA)** module  
  → Preserves both high- and low-frequency signal components  
- ✅ Enhances long-horizon stability of Transformers  
- ✅ Provides significant improvements in MSE and MAE  
- ✅ Architecture-agnostic improvement  
  → Can be added to Informer, Autoformer, etc.

---

## 🧪 Methodology
| Component | Description |
|----------|-------------|
| BFA block | Controls frequency attenuation across layers |
| FFT-based frequency decomposition | Extracts multi-frequency signal components |
| Plug-and-play design | Can integrate with existing TS Transformers |

Key insight:
💡 **Transformers tend to lose high-frequency signal features** over long horizons → BEAT reduces this degradation.

---

## 📈 Results
Evaluated on benchmarks such as:
- ETT (Electricity Transformer Temperature)
- Weather
- Traffic

| Model | Improvement with BEAT |
|-------|---------------------|
| Informer | +8–12% |
| Autoformer | +5–10% |

Performance gains **increase as forecasting horizon grows** ✅

---

## ✅ Strengths
- State-of-the-art for **long-horizon TS forecasting**
- Improves robustness of Transformer architectures
- Computationally efficient module

---

## ⚠️ Limitations
- Primarily focused on synthetic + benchmark datasets
- Limited validation in real-world infrastructure systems
- Interpretability remains minimal

---

## 🤝 Relevance to CAST Project
✔
