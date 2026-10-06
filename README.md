# Network Intrusion Detection System

A machine learning project for **network intrusion detection** using tabular network-traffic data. The objective is to distinguish normal network activity from potentially malicious or anomalous traffic and provide a reproducible classification workflow.

## Project Overview

Network Intrusion Detection Systems (NIDS) monitor network traffic and use traffic characteristics to identify suspicious activity. Machine learning can automate this process by learning patterns associated with normal and malicious network behaviour.

The main implementation is provided in **`project_1(network_intrution).ipynb`**.

## Repository Contents

| File | Description |
|---|---|
| `project_1(network_intrution).ipynb` | Main notebook containing the intrusion-detection analysis and modelling workflow |
| `training_project_1.parquet` | Training dataset |
| `testing_project_1.parquet` | Testing dataset |
| `README.md` | Project documentation |
| `.ipynb_checkpoints/` | Jupyter Notebook checkpoint files |

## Workflow

The project follows an end-to-end machine learning workflow for network-security classification:

1. **Load network-traffic data** from the supplied Parquet files.
2. **Inspect and explore the dataset**, including feature types, distributions and target classes.
3. **Preprocess the traffic features** for machine learning.
4. **Prepare training and testing data** using the provided dataset split.
5. **Train classification models** to learn patterns associated with network intrusions.
6. **Evaluate predictions** using classification-oriented performance measures.
7. **Analyse model behaviour** and the resulting intrusion-detection performance.

## Data

The repository contains separate Parquet files for training and testing:

- `training_project_1.parquet`
- `testing_project_1.parquet`

Keeping the training and testing datasets separate makes it possible to evaluate the trained models on data that was not used during model fitting.

> **Note:** The dataset files are included for reproducibility. Their size may require several gigabytes of available storage/RAM depending on how the notebook loads and processes them.

## Technologies

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- scikit-learn
- PyArrow / Parquet

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yuvraj619/Network_intrusion_detection_system.git
cd Network_intrusion_detection_system
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib scikit-learn pyarrow jupyter
```

### 3. Run the notebook

```bash
jupyter notebook "project_1(network_intrution).ipynb"
```

Run the notebook cells sequentially to reproduce the analysis.

## Why Intrusion Detection Matters

Traditional security systems rely heavily on predefined rules and signatures. Machine learning-based intrusion detection can complement these approaches by learning statistical patterns in traffic and potentially identifying previously unseen or evolving behaviours.

A useful NIDS therefore needs to balance:

- Detection capability
- False-positive rate
- Generalisation to unseen traffic
- Computational efficiency
- Robustness against changing attack patterns

## Key Learning Objectives

- Apply machine learning to a cybersecurity problem.
- Work with structured network-traffic data.
- Build a binary/multiclass classification workflow.
- Understand preprocessing for security datasets.
- Evaluate intrusion-detection models appropriately.
- Consider the practical trade-off between detecting attacks and generating false alarms.

## Limitations

This project is intended for learning and experimentation. A production NIDS would require additional work such as real-time traffic ingestion, feature extraction, model monitoring, adversarial robustness testing, threshold calibration, drift detection and continuous validation on representative network traffic.

## Author

**Yuvraj Arora**  
GitHub: [@yuvraj619](https://github.com/yuvraj619)

---

This project is part of an ongoing machine learning and applied AI portfolio.