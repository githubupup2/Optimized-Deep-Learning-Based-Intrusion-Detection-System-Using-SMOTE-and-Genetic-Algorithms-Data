# Optimized-Deep-Learning-Based-Intrusion-Detection-System-Using-SMOTE-and-Genetic-Algorithms-Data
Optimized Deep Learning-Based Intrusion Detection System Using SMOTE and Genetic Algorithms paper

This repository contains the lightweight version of the **NCST-IDS2025** dataset, designed to support the reproduction of our intrusion detection experiments based on **SMOTE** oversampling and **Genetic Algorithm (GA)** optimization. The original dataset is very large (several gigabytes), so we release a condensed version for quick experimentation and validation.

---

## 📌 Dataset Description

- 📊 **Features**: 87 numerical features representing network traffic behavior.
- 🏷️ **Label column**: `label`, with 5 representative attack types:
  - `DoS`
  - `CommandInjection`
  - `BufferOverflow`
  - `DenialOfService`
  - `Repudiation`
- 📦 **Samples**: 2,500 per class (total: 12,500 rows).
- 🌐 **Scenario column**: Indicates the context (e.g., IoT, IIoT, V2X), available for scenario-specific studies.

---

## 🔍 Usage

### 1. Clone the repo and load data:
```python
import pandas as pd

df = pd.read_csv("ncst_ids2025_full.csv")
print(df.shape)
print(df['label'].value_counts())
