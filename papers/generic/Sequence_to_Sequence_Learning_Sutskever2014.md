# Sequence to Sequence Learning with Neural Networks (2014)

📄 Paper Link: https://arxiv.org/abs/1409.3215  
📂 Local PDF: ../../1409.3215v3.pdf  
✍️ Authors: Sutskever, Vinyals & Le  
🏫 Published in: NeurIPS 2014  

---

## 🎯 Objective
Introduce a **general sequence-to-sequence learning framework** using **two LSTM networks** (Encoder + Decoder) to perform machine translation and other sequence prediction tasks.

---

## 🧠 Key Contributions
- ✅ Introduced the **Encoder–Decoder** architecture
- ✅ Demonstrated strong performance in **machine translation**
- ✅ Showed that **sequence lengths can differ** between input/output
- ✅ Introduced key technique: **Reverse input sequence → +improves learning**

---

## 🧪 Methodology
| Component | Role |
|----------|------|
| Encoder LSTM | Encodes full input sequence into a vector |
| Decoder LSTM | Generates output sequence step-by-step |
| Teacher forcing | Helps learning during training |

Key idea:
- Encoder compresses the entire sequence into a **fixed-length vector**
- Decoder **reconstructs** the sequence from that vector

⚠️ Limitation: Bottleneck when sequences are long.

---

## 📈 Results
- Improved BLEU scores vs. previous MT systems
- First successful demonstration of **end-to-end learned translation**
- Established foundation for all **modern autoregressive models**

---

## ✅ Strengths
- Handles **variable-length** sequences
- Works well for short-to-moderate horizons
- Clear and elegant architecture

---

## ⚠️ Limitations
- Memory bottleneck → struggles with **long sequences**
- No attention → decoder lacks direct access to full input sequence
- Training can be slow

---

## 🤝 Relevance to CAST Project
✔ Base conceptual framework for sequence forecasting  
✔ Helps contextualizar **por que razão** Transformers surgiram  
✔ Será importante na tua Revisão de Literatura como **ponto histórico**  
✔ Bom baseline para comparação de resultados com o CAST

---

## 🔍 Tags
Seq2Seq • LSTM • Encoder–Decoder • Sequence Modeling
