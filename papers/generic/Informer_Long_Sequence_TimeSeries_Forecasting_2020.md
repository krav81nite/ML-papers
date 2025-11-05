# Informer: Beyond Efficient Transformer for Long Sequence Time-Series Forecasting (2020)

📄 Paper Link: https://arxiv.org/abs/2012.07436  
📂 Local PDF: ../../2012.07436v3.pdf  
✍️ Authors: Zhou et al.  
🏫 Published in: AAAI 2021  

---

## 🎯 Objective
Address the **quadratic complexity** of attention in Transformers and improve long sequence forecasting tasks through:

- **Efficient attention mechanisms**
- Better handling of **long-term dependencies**

---

## 🧠 Key Contributions
- ✅ **ProbSparse Self-Attention**  
  → selects only *dominant queries*  
  → reduces complexity from O(L²) ➝ O(L log L)
- ✅ **Self-Attention Distilling**  
  → gradually compresses long sequences (pyramid-like)
- ✅ **Generative Decoder**  
  → predicts full horizon in *one forward pass*

⬆️ This makes Informer **fast and scalable** for long-term forecasting.

---

## 🧪 Methodology

| Component | Function |
|----------|----------|
| Encoder with distillation | Compress time dimension while keeping key signals |
| ProbSparse Attention | Efficient long-range pattern capture |
| Auto-regressive vs Generative outputs | Enables multi-step forecasting |

Framework goal:
💡 Preserve essential information while reducing compute.

Datasets used:
- ETT (Electricity Transformer Temperature)
- Weather
- Exchange
- Traffic

---

## 📈 Results

| Model | Long-Horizon Performance |
|-------|-------------------------|
| Informer | ⭐ Significant improvement vs LSTM/Transformer |
| Transforme
