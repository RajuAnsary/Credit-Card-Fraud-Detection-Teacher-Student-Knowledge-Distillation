# Credit Card Fraud Detection Using Teacher–Student Knowledge Distillation

## Project Overview

This project presents a hybrid machine learning framework for credit card fraud detection using **Teacher–Student Knowledge Distillation**. The proposed approach combines a **Graph Attention Network v2 (GATv2)** as the Teacher model and a lightweight **SE-ResNet** as the Student model to achieve high fraud detection performance while maintaining fast inference speed.

The framework is evaluated on **two publicly available Kaggle datasets** and compared against **XGBoost** and **Plain MLP** baseline models using multiple evaluation metrics.

---

## Key Features

- Hybrid Teacher–Student Knowledge Distillation framework
- Graph-based fraud detection using **GATv2**
- Lightweight **SE-ResNet Student** for fast inference
- Graph construction using **k-Nearest Neighbors (k-NN)** and cosine similarity
- BorderlineSMOTE for handling class imbalance
- Probability calibration and threshold optimization
- Cross-dataset evaluation on two public fraud datasets
- Performance comparison with XGBoost and Plain MLP
- Optional model explainability using SHAP

---

# Proposed Methodology

The proposed framework consists of the following stages:

1. Data Loading
2. Data Cleaning
3. Train / Validation / Test Split
4. Target Encoding
5. Quantile Transformation
6. BorderlineSMOTE
7. Graph Construction using k-NN
8. Teacher Model (GATv2)
9. Student Model (SE-ResNet)
10. Knowledge Distillation
11. Teacher–Student Ensemble
12. Probability Calibration
13. Threshold Optimization
14. Performance Evaluation

---

# Project Pipeline

```
Input Datasets
        │
        ▼
Load & Clean Data
        │
        ▼
Train / Validation / Test Split
        │
        ▼
Preprocessing
(Target Encoding + Quantile Transformation + BorderlineSMOTE)
        │
        ▼
Graph Construction (k-NN + Cosine Similarity)
        │
 ┌──────┴─────────────┐
 │                    │
 ▼                    ▼
Teacher (GATv2)   XGBoost (Baseline)
 │
 ▼
Knowledge Distillation
 │
 ▼
Student (SE-ResNet)
 │
 ▼
Teacher + Student Ensemble
 │
 ▼
Calibration & Threshold Optimization
 │
 ▼
Performance Evaluation
```

---

# Models Used

### Teacher Model

- Graph Attention Network v2 (GATv2)

### Student Model

- SE-ResNet

### Baseline Models

- XGBoost
- Plain Multi-Layer Perceptron (MLP)

### Ensemble Model

- Weighted combination of Teacher and Student predictions

---

# Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- PR-AUC
- Matthews Correlation Coefficient (MCC)
- Balanced Accuracy
- Cohen's Kappa

---



# Technologies Used

- Python
- PyTorch
- Torch-Geometric
- Scikit-learn
- XGBoost
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SHAP

---

# Installation



Install dependencies

```bash
pip install -r requirements.txt
```

For Google Colab

```bash
pip install imbalanced-learn xgboost shap torch-geometric
```

---

# How to Run

1. Open the Jupyter Notebook or Google Colab notebook.
2. Upload the two dataset files when prompted.
3. Run all notebook cells sequentially.
4. View ROC, PR curves, confusion matrices, and benchmark results.

---


# Future Work

- Real-time fraud detection system
- Temporal Graph Neural Networks
- Explainable AI using SHAP and Attention Visualization
- Federated Learning
- Online Learning for concept drift
- Deployment as REST API using FastAPI

---

# Authors

- **Raju Ansary**
- **Moupriyo Jana**


---

# License

This project is developed for academic and research purposes.
