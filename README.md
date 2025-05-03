# Botnet Detection using Hybrid LSTM-Attention Model

## 📌 Project Overview

This project focuses on detecting botnet-related Distributed Denial-of-Service (DDoS) attacks using a deep learning-based approach. A hybrid architecture combining a Bidirectional LSTM and a Self-Attention mechanism is employed to effectively learn temporal patterns and highlight crucial time-step features in network traffic data.

---

## ❓ What is a Botnet?

A **botnet** is a network of compromised devices that are remotely controlled by malicious actors. These devices can be used to:
- Launch **DDoS attacks**
- Perform **data theft**
- Run **spam campaigns**
- Carry out other **unauthorized activities** without the user's knowledge

---

## ⚠️ Why is Detection Important?

- **Severe Cybersecurity Threats**: Botnets lead to data breaches, infrastructure damage, and financial loss.
- **DDoS Attacks**: They flood target servers, causing downtime and disrupting services.
- **Compromised Devices**: Exploited silently, leading to privacy violations and resource misuse.

---

## 📊 Dataset

**CIC-DDoS2019**  
A benchmark dataset for detecting Distributed Denial-of-Service attacks. It contains:
- Real-world network traffic
- Multiple types of DDoS attacks
- Benign traffic for baseline comparisons

[Dataset Source](https://www.unb.ca/cic/datasets/ddos-2019.html)

---

## 🧠 Model Architecture: Hybrid LSTM-Attention

### 🔄 Bidirectional LSTM
- Captures long-term temporal dependencies from both past and future sequences.

### 🎯 Self-Attention Mechanism
- Computes attention weights across LSTM outputs.
- Focuses on critical time steps by enhancing important features.

### 🔁 Residual Connection
- Combines raw LSTM output with attention-enhanced features.
- Preserves information and improves gradient flow.

### 🔧 Feature Processing
- Global Average Pooling
- Fully Connected Layers
- Batch Normalization
- Dropout for generalization

### 🧪 Classification Head
- Output layer uses **Softmax activation** to predict traffic classes.

---

## 🛠️ Setup Instructions

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/botnet-detection-lstm-attention.git
   cd botnet-detection-lstm-attention
