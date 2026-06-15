# CS2205.CH203-UAV-TWIN-GRAPH-ADA

## 📝 Project Overview
This repository contains the official implementation of an advanced Intrusion Detection System (IDS) for Unmanned Aerial Vehicle (UAV) networks. The project proposes a novel deep learning framework that enhances network resilience against evolving cybersecurity threats and concept drift under severe data scarcity constraints.

### 🌟 Key Innovations & Methodology
Our approach bridges the structural context of network traffic with domain-adversarial generalization:

1. **Twin Graph Architecture:** Following the principles of Xue Li et al. `[1]`, we extract and split raw network packets into **Header** and **Payload**. These components are transformed into complementary graph representations—**Co-occurrence Graphs** and **Word Frequency Graphs**—to preserve full semantic and spatial context.
2. **Structural Feature Extraction:** We integrate a **Graph Isomorphism Network (GIN)** combined with a **Global Attention Pooling** mechanism to dynamically weight and aggregate expressive node embeddings into robust graph-level vectors.
3. **Adversarial Domain Adaptation (ADA):** To tackle the challenge of malware evolution and concept drift with minimal samples `[2, 3]`, an adversarial framework (comprising a *Task Classifier* and a *Domain Discriminator*) is deployed. This forces the model to learn drift-invariant features, enabling high-accuracy detection on new attack variants even with extremely limited labeled target data.

### 📊 Dataset & Evaluation
The model is evaluated on **UAV-NIDD** `[4]`, a dynamic and specialized dataset for drone cybersecurity. Experimental setups demonstrate that our framework maintains outstanding detection accuracy (Accuracy and F1-score) while significantly reducing computational overhead and processing latency, making it highly feasible for resource-constrained UAV hardware.

### [Report Presentation Video](https://youtu.be/yInmyjniRpI?si=SNUNGRJyocLH3IWy)

By:
Nguyen Pham Uyen Thi - 250202055
---

## 📚 References
* `[1]` Xue Li, Ting Zhang, Jun Wang, Jie Nie, et al. "Enhance UAV Network Resilience by Malicious Traffic Detection: A Twin Graph Encoder Approach." *IEEE Transactions on Communications*, 2026.
* `[2]` J. Zhang et al. "Revisiting concept drift in windows malware detection: Adaptation to real drifted malware with minimal samples." *IEEE Transactions on Information Forensics and Security*, vol. 19, pp. 1104–1117, 2024.
* `[3]` Y. Ganin et al. "Domain-adversarial training of neural networks." *Journal of Machine Learning Research*, vol. 17, no. 1, pp. 2096–2030, 2016.
* `[4]` Hadi J. Hadi et al. "UAV-NIDD: A Dynamic Dataset for Cybersecurity and Intrusion Detection in UAV Networks." *IEEE Transactions on Network Science and Engineering*, 12(4): 2739-2757 (2025).
