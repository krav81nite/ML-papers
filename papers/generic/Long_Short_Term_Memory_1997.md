# Long Short-Term Memory (1997)

📄 Paper Link: https://www.bioinf.jku.at/publications/older/2604.pdf  
📂 Local PDF: ../../2604.pdf  
✍️ Authors: Hochreiter & Schmidhuber  
🏫 Published in: Neural Computation, 1997  

---

## 🎯 Objective
Solve the **vanishing/exploding gradient problem** in RNNs, enabling learning of **long-term temporal dependencies** that standard recurrent networks fail to capture.

---

## 🧠 Key Contributions
- ✅ Proposes the **LSTM** architecture
- ✅ Introduces **memory cells** that preserve information over long time periods
- ✅ Introduces **input, output, and forget gates** to control memory flow
- ✅ Demonstrates improved learning stability in sequential tasks

---

## 🧪 Methodology

| Component | Function |
|----------|----------|
| Memory Cell | Stores long-term state |
| Input Gate | Controls new information entering memory |
| Forget Gate | Removes outdated information |
| Output Gate | Produces hidden output |

Key equation form (simplified):

\[
c_t = f_t \odot c_{t-1} + i_t \odot \tilde{c_t}
\]

💡 The *forget gate* is crucial for sequence modeling.

---

## 📈 Results
Successfully learns tasks that standard RNNs **could not**:
- Long-distance temporal relationships
- Time-lag dependency benchmarks

Performance showed major advancements over:
- Vanilla RNNs
- Simple recurrent networks (SRNs)

---

## ✅ Strengths
- Solves gradient vanishing/exploding issues
- Excellent for **short to medium** forecasting horizons
- Very adaptable architecture

---

## ⚠️ Limitations
- Still **sequential computation** → slow training
- Struggles with **very long sequences**
- High parameter count → comput
