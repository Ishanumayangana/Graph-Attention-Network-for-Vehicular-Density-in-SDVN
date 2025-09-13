# 🚗 Graph Attention Network for Vehicular Density in SDVN

This project implements a **Graph Attention Network (GAT)** to model and predict
vehicular density–related parameters in **Software-Defined Vehicular Networks (SDVN)**.
It is designed to run in **Google Colab** using **PyTorch Geometric**.

The model learns from node-level features (vehicular density, speed, acceleration, etc.)
and predicts link reliability / path quality as a supervised task.

---

## 📌 Project Overview

- **Input Graph**
  - Nodes: vehicles with features such as position, speed, acceleration, local density.
  - Edges: built using k-nearest neighbor (kNN) or communication range (connectivity).
- **Model**
  - Multi-layer, multi-head **Graph Attention Network (GAT)**.
  - Node-level supervised regression task (predicting link reliability).
- **Outputs**
  - Predicted reliability scores for each vehicle node.
  - Training and validation loss curves.
  - 2D scatter plots of actual vs predicted reliability.

---

## ⚙️ Features

- Colab-ready, cell-by-cell notebook.
- Synthetic SDVN dataset generator (can be replaced with real SDVN data).
- Train/Val/Test masks for supervised training.
- GAT model with adjustable layers, heads, and hidden dimensions.
- Training, evaluation, and visualization utilities.

