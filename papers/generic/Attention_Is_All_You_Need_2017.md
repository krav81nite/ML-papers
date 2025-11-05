# Attention Is All You Need (2017)

📄 Paper Link: https://arxiv.org/abs/1706.03762  
📂 Local PDF: ../../1706.03762v7.pdf  
✍️ Authors: Vaswani et al.  
🏫 Published in: NeurIPS 2017  

---

## 🎯 Objective
Introduce a novel neural network architecture for sequence modeling that **replaces recurrence** entirely using **self-attention**, achieving better parallelization and long-range dependency learning.

---

## 🧠 Key Contributions
- ✅ Introduced the **Transformer** architecture  
- ✅ Proposed **Multi-Head Self-Attention** mechanism  
- ✅ Removed recurrence → **fully parallelizable**  
- ✅ Achieved state-of-the-art performance in machine translation  
- ✅ Laid the foundation for modern LLMs (BERT, GPT, T5…)

---

## 🧪 Methodology
| Component | Description |
|----------|-------------|
| Architecture | Encoder–Decoder |
| Core Mechanism | Scaled Dot-Product Self-Attention |
| Positional Encoding | Injects notion of temporal order |
| Optimization | Adam with warm-up learning rate |

Key formula:
\[
\text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V
\]

The model learns which parts of the sequence to **attend** to when predicting the next step.

---

## 📈 Results
- Outperformed previous **Seq2Seq with LSTM** in translation tasks
- Required **significantly less training time**
- Enabled modeling long contexts more efficiently than RNN-based models

| Model | BLEU Score | Training Speed |
|-------|------------|----------------|
| LSTM Seq2Seq | Lower | Slow |
| Transformer | ⭐ Higher | ⭐ Much Faster |

---

## ✅ Strengths
- Efficient for **long-range** sequence dependencies  
- Highly parallelizable → faster inference and training  
- Flexible architecture → adapts to many domains (text, time series, vision…)  

---

## ⚠️ Limitations
- Complexity can grow **quadratically** with sequence length  
- Requires **positional encoding** to retain order  
- For very long time series → may require optimized variants (ex.: Informer)  

---

## 🤝 Relevance to CAST Project
✔ Ideal for **predicting sequential patterns** in EV charging availability  
✔ Can capture **daily/weekly cyclic usage**  
✔ Enables adding **contextual inputs** (time of day, location, events…)  
✔ A strong baseline to compare against LSTM and classical models  

---

## 🔍 Tags
Transformers • Self-Attention • Sequence-to-Sequence • Deep Learning

