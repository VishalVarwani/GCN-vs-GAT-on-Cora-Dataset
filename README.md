# 🔥 Graph Neural Networks: GCN vs. GAT on Cora Dataset  

### 🚀 **What’s This Project About?**  
In this project, we **compare two powerful Graph Neural Networks (GNNs)**—**Graph Convolutional Networks (GCN) and Graph Attention Networks (GAT)**—on the **Cora dataset** to see which one performs better in node classification.  

### 🤔 **Why This Project?**  
Graph data is **everywhere**—social networks, recommendation systems, biology, etc. But traditional ML models **struggle with graphs** because they assume data is independent, which isn’t true in graphs. GNNs fix this by learning **relationships between connected nodes**.  

This project asks a simple question:  
💡 **Is it better to treat all connections equally (GCN) or assign different importance to different connections (GAT)?**  

---

## 📌 **The Dataset: Cora (Why This One?)**
Cora is a classic benchmark dataset for graph learning. It consists of:  
- **2,708 nodes** (academic papers)  
- **5,429 edges** (citations between papers)  
- **7 classes** (paper topics like AI, NLP, etc.)  
- Each node (paper) has **1,433 features** (word embeddings)  

We use Cora because **it’s small but complex enough to show real differences between GNN models**.

---

Why Train for 200 Epochs?
GNNs take time to learn node embeddings properly.
Too few epochs = underfitting (model doesn’t learn enough).
Too many epochs = overfitting (model memorizes training data).
200 epochs was chosen based on convergence trends—after ~150 epochs, both models stabilized.

Model	Test Accuracy (%)
Final GCN Test Accuracy: 81.60%
Final GAT Test Accuracy: 68.20%

