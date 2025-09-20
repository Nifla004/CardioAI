## CardioAI: Anomaly Detection in ECG Data
CardioAI is a research-oriented project for detecting anomalies in ECG-like data using Isolation Forest and Autoencoder models. The project is inspired by a real-life case of unexplained pericardial effusion and explores AI/ML techniques for cardiac anomaly detection.

### Motivation
Early detection of cardiac anomalies is critical for preventing severe cardiovascular events. Traditional ECG analysis requires expert interpretation. CardioAI automates anomaly detection, making it useful for clinical decision support and research.

### Features
- Synthetic ECG-like data generation for normal and anomalous patterns.
- Isolation Forest for unsupervised anomaly detection.
- Autoencoder for reconstructing normal ECG patterns and detecting anomalies.
- Evaluation metrics: Precision, Recall, F1-Score, ROC-AUC.
- Visualizations of anomaly scores and reconstruction errors.

### Folder Structure
CardioAI/
├─ notebooks/ # Colab/Jupyter notebooks
│ └─ CardioAI_notebook.ipynb
├─ paper/ # Research paper PDF
│ └─ CardioAI_research_paper.pdf
├─ README.md # Project overview

### How to Run
1. Open `CardioAI_notebook.ipynb` in Google Colab or Jupyter.  
2. Run all cells sequentially to generate metrics, results, and plots.  
3. Modify dataset or parameters if needed.  
4. Review comparison tables and visualization outputs.

### Dependencies
- Python 3.x  
- numpy, pandas, matplotlib, scikit-learn, tensorflow (keras)  
Install missing packages using:
pip install numpy pandas matplotlib scikit-learn tensorflow

### Methodology
- **Synthetic Data:** Generated using Gaussian distributions for normal and anomalous ECG-like signals.  
- **Isolation Forest:** Unsupervised model trained on full dataset. Predictions converted (-1 → anomaly, 1 → normal). Evaluated with precision, recall, F1-score, ROC-AUC.  
- **Autoencoder:** Feedforward neural network trained only on normal data. Reconstruction error computed for all samples. Threshold = mean + 3*std of normal error. Samples above threshold classified as anomalies.  
- **Comparison:** Both models evaluated on same dataset; results compared via metrics and visualizations.

### Results
| Model             | Precision | Recall | F1-Score | ROC-AUC |
|------------------|-----------|--------|----------|---------|
| Isolation Forest  | 0.943     | 1.000  | 0.971    | 0.998   |
| Autoencoder       | 0.877     | 1.000  | 0.935    | 0.996   |

**Observation:** Both models detect anomalies effectively. Isolation Forest has slightly higher precision, Autoencoder achieves perfect recall. Visualizations show clear separation between normal and anomalous samples.

### Visualizations
- Isolation Forest: Histogram of anomaly scores.  
- Autoencoder: Histogram of reconstruction errors with threshold line.

### References
- [Isolation Forest Paper](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/icdm08b.pdf)  
- [Autoencoder-based Anomaly Detection](https://arxiv.org/abs/1802.04410)

### Author
Nifla Nalakath, Department of Computer Science and Engineering, Eranad Knowledge City Technical Campus (EKCTC), APJ Abdul Kalam Technological University (KTU)
