# A Novel CNN-BiLSTM Model with Multi-Head Attention for Efficient Intrusion Detection

<p align="center">
  <strong>An IEEE COMPAS 2025 Research Project</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Conference-IEEE-blue?style=for-the-badge&logo=ieee" />
  <img src="https://img.shields.io/badge/Domain-Cybersecurity-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Deep%20Learning-CNN--BiLSTM-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Attention-Multi--Head-purple?style=for-the-badge" />
</p>

## 📌 Overview

This repository contains the implementation of our research paper, **"A Novel CNN-BiLSTM Model with MultiHead Attention for Efficient Intrusion Detection,"** published at the IEEE 2nd International Conference on Computing, Applications and Systems (COMPAS 2025).

The research proposes a hybrid deep learning architecture combining Convolutional Neural Networks (CNN), Bidirectional Long Short-Term Memory (BiLSTM), and Multi-Head Attention (MHA) to improve network intrusion detection.

The proposed approach aims to identify malicious network traffic by extracting important network features, learning sequential patterns, and focusing on relevant feature representations through attention mechanisms.

The model is evaluated using two benchmark cybersecurity datasets:

- UNSW-NB15
- NSL-KDD

## 🎯 Research Objectives

- Develop a hybrid CNN-BiLSTM architecture for network intrusion detection.
- Extract meaningful network traffic features using CNN layers.
- Capture sequential dependencies using BiLSTM.
- Apply Multi-Head Attention to enhance feature representation.
- Distinguish between normal and malicious network traffic.
- Evaluate model performance across two benchmark intrusion detection datasets.

## 🧠 Proposed Model Architecture

The proposed architecture integrates three major deep learning components:

**1. Convolutional Neural Network (CNN)**

Extracts important spatial and local patterns from network traffic features using convolutional layers.

**2. Bidirectional Long Short-Term Memory (BiLSTM)**

Captures sequential dependencies and contextual information from network traffic in both forward and backward directions.

**3. Multi-Head Attention (MHA)**

Enhances feature representation by allowing the model to focus on relevant information and capture contextual relationships.

### Architecture Workflow

```text
Network Traffic Dataset
          |
          v
 Data Preprocessing
          |
          v
   CNN Feature Extraction
          |
          v
  Feature Representation
          |
          v
 Multi-Head Attention
          |
          v
     BiLSTM Layer
          |
          v
   Dense Classification
          |
          v
   Normal / Malicious
```

## 📊 Datasets

The proposed model was evaluated using two publicly available benchmark datasets.

| Dataset | Total Samples | Training | Validation | Testing |
|---|---:|---:|---:|---:|
| UNSW-NB15 | 257,669 | 180,368 | 38,650 | 38,651 |
| NSL-KDD | 125,973 | 88,181 | 18,896 | 18,896 |

### 1. UNSW-NB15

UNSW-NB15 contains normal network traffic and multiple attack categories, including DoS, backdoors, and exploits.

### 2. NSL-KDD

NSL-KDD is a benchmark intrusion detection dataset containing normal traffic and several attack categories, including DoS, Probe, Remote to Local (R2L), and User to Root (U2R).

**Dataset distribution:** 70% training, 15% validation, and 15% testing.

## ⚙️ Model Configuration

The proposed CNN-BiLSTM architecture includes:

- Conv1D layers with 64 and 128 filters.
- ReLU activation.
- Batch Normalization.
- Max Pooling (pool size 2).
- Dropout (0.4).
- Multi-Head Attention mechanism.
- BiLSTM layer with 64 units.
- Dense classification layers.
- Sigmoid activation for binary classification.

## 📈 Experimental Results

The proposed model achieved the following test accuracies:

| Dataset | Model | Test Accuracy |
|---|---|---:|
| NSL-KDD | CNN-BiLSTM | **98.96%** |
| UNSW-NB15 | Hybrid CNN-BiLSTM | **99.99%** |

### Performance Evaluation

The research evaluates the model using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- Training and Validation Accuracy
- Training and Validation Loss

### Visualizations

The research includes:

- Dataset correlation heatmaps.
- Feature importance visualizations.
- Proposed model architecture.
- System workflow diagram.
- Training and validation accuracy curves.
- Training and validation loss curves.
- Confusion matrix.
- Classification report.

## 🛠️ Technologies

The implementation uses Python-based machine learning and deep learning tools.

- Python
- Deep Learning
- Convolutional Neural Networks (CNN)
- Bidirectional LSTM (BiLSTM)
- Multi-Head Attention
- Network Intrusion Detection
- Data Preprocessing
- Data Visualization

## 📁 Repository Structure

```text
CNN-BiLSTM-Intrusion-Detection/
│
├── README.md
│
├── notebooks/
│   ├── UNSW_NB15.ipynb
│   └── NSL_KDD.ipynb
│
├── results/
│   ├── confusion_matrix.png
│   ├── accuracy.png
│   └── loss.png
│
└── requirements.txt
```

*Note: The structure above is illustrative. Adjust the filenames and folders to match the actual repository.*

## 🚀 Getting Started

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd YOUR_REPOSITORY_NAME
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Select the relevant dataset notebook and follow the execution steps.

*Ensure that the required datasets are downloaded and placed in the paths specified in the notebooks.*

## 📄 Research Publication

**Paper Title:** A Novel CNN-BiLSTM Model with MultiHead Attention for Efficient Intrusion Detection

**Conference:** IEEE 2nd International Conference on Computing, Applications and Systems (COMPAS 2025)

**Conference Date:** 23–24 October 2025

**DOI:** [10.1109/COMPAS67506.2025.11381796](https://doi.org/10.1109/COMPAS67506.2025.11381796)

**Publisher:** IEEE

## 👨‍💻 Authors

- Omar Hasnain Mahmud
- **Abdullah Al Noman**
- Mohammad Nadib Hasan
- Md Jiabul Hoque
- Abdullah Al Afiq

## 📚 Citation

If you use this research in your work, please cite the original publication:

```bibtex
@inproceedings{mahmud2025novel,
  title={A Novel CNN-BiLSTM Model with MultiHead Attention for Efficient Intrusion Detection},
  author={Mahmud, Omar Hasnain and
          Al Noman, Abdullah and
          Hasan, Mohammad Nadib and
          Hoque, Md Jiabul and
          Al Afiq, Abdullah},
  booktitle={2025 IEEE 2nd International Conference on
             Computing, Applications and Systems (COMPAS)},
  year={2025},
  doi={10.1109/COMPAS67506.2025.11381796}
}
```

## 🔬 Future Research

Potential directions for further research include:

- Improving detection of previously unseen cyberattacks.
- Evaluating generalization across different network environments.
- Optimizing computational efficiency for real-time intrusion detection.
- Exploring more advanced attention mechanisms.
- Investigating class imbalance and evolving attack patterns.

## ⭐ Acknowledgements

This work was conducted as a collaborative research project in the field of deep learning and network cybersecurity.

If you find this research useful, consider starring ⭐ this repository.

---

**Research Area:** Deep Learning | Cybersecurity | Network Intrusion Detection | Attention Mechanisms | CNN-BiLSTM
