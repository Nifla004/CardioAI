# CardioAI: Cardiac Anomaly Detection using Isolation Forest and Autoencoder

CardioAI is a research-oriented machine learning project for detecting cardiac anomalies from ECG-inspired clinical data using unsupervised anomaly detection techniques.

The project was inspired by a real-life case of unexplained pericardial effusion and investigates how artificial intelligence can assist in identifying abnormal cardiac patterns when conventional diagnosis is challenging.

---

# Motivation

Early detection of cardiac abnormalities can significantly improve clinical outcomes. Traditional diagnostic methods may fail to identify rare or unexplained cardiac conditions in their early stages.

CardioAI explores the use of unsupervised machine learning models capable of learning normal cardiac behaviour and detecting anomalous patterns without requiring extensive labelled datasets.

---

# Objectives

- Detect cardiac anomalies using Artificial Intelligence.
- Compare two anomaly detection models.
- Evaluate model performance using standard metrics.
- Demonstrate the applicability of AI for early cardiac anomaly detection.
- Provide a reproducible research framework for future healthcare AI studies.

---

# Models Used

## Isolation Forest

- Unsupervised anomaly detection
- Tree-based ensemble algorithm
- Detects abnormal cardiac patterns using anomaly scores

## Autoencoder

- Deep learning reconstruction model
- Learns normal cardiac behaviour
- Detects anomalies using reconstruction error

---

# Dataset

The project uses ECG-inspired clinical data generated for anomaly detection experiments.

Normal and anomalous cardiac samples are prepared for evaluating unsupervised learning methods.

---

# Methodology

1. Data preprocessing
2. Feature scaling
3. Isolation Forest training
4. Autoencoder training
5. Anomaly score calculation
6. Reconstruction error analysis
7. Model evaluation
8. Performance comparison

---

# Evaluation Metrics

The models are evaluated using:

- Precision
- Recall
- F1 Score
- ROC-AUC

---

# Results

| Model | Precision | Recall | F1 Score | ROC-AUC |
|--------|----------:|-------:|---------:|---------:|
| Isolation Forest | 0.943 | 1.000 | 0.971 | 0.998 |
| Autoencoder | 0.877 | 1.000 | 0.935 | 0.996 |

### Observation

- Isolation Forest achieved the highest overall performance.
- Autoencoder achieved perfect recall, detecting all anomalous samples.
- Both models demonstrated excellent capability for cardiac anomaly detection.

---

# Visualizations

The project includes:

- Isolation Forest anomaly score distribution
- Autoencoder reconstruction error distribution
- ROC Curve
- Confusion Matrix
- Performance comparison charts

---

# Project Structure

```
CardioAI
│
├── notebooks/
│   └── CardioAI.ipynb
│
├── paper/
│   └── CardioAI_Research_Paper.pdf
│
├── figures/
│
├── README.md
│
└── LICENSE
```

---

# Installation

Install the required packages:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow
```

---

# How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Install the required dependencies.
3. Run all cells sequentially.
4. Review the evaluation metrics and visualizations.

---

# Future Work

Future development will extend CardioAI into **CardioAI+**, which will include:

- Explainable AI (SHAP)
- Streamlit Clinical Dashboard
- Clinical Decision Support
- Batch Prediction
- Model Comparison
- Support for multiple heart-related datasets

---

# References

- Isolation Forest
- Autoencoder-based Anomaly Detection
- Scikit-learn Documentation
- TensorFlow/Keras Documentation

---

# Author

**Nifla Nalakath**

Department of Computer Science and Engineering

Eranad Knowledge City Technical Campus (EKCTC)

APJ Abdul Kalam Technological University (KTU)

---

## License

This project is developed for academic and research purposes.