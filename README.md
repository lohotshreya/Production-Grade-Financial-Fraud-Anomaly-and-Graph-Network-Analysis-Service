# Structural Outlier Detector: Financial Fraud & Network Anomaly Engine

An unsupervised machine learning and network graph analytics pipeline designed to isolate systemic anomalies and coordinated fraudulent structures within dense transaction ledgers. This repository implements an end-to-end engineering solution for processing high-cardinality financial interaction logs, extracting statistical outliers, and mapping multi-node structural risk.

---

## System Architecture

Unlike traditional supervised classifiers that rely on static, pre-labeled historical data, this system operates entirely on an **unsupervised paradigm**, optimizing it for real-world corporate environments where fraudulent vectors are highly dynamic and anomalies represent less than 0.1% of total transaction volumes.



The architecture executes across three distinct core layers:
1. **The Vector Engine (Isolation Forest):** Isolates extreme behavioral multi-dimensional anomalies (transaction frequency anomalies, sudden volume velocity shifts, spatial time-delta anomalies).
2. **The Topological Pipeline (NetworkX Graphs):** Maps high-risk transaction interactions as graph nodes and directional edges, isolating multi-account structuring rings or funnel networks.
3. **The Analytics Front-End (Streamlit/Plotly):** Translates complex mathematical anomaly matrices into an intuitive, high-end production dashboard for fraud operators.

---

## Tech Stack & Engineering Toolkit

* **Core Analytics & Math:** Python, NumPy, Pandas
* **Unsupervised Machine Learning:** Scikit-Learn (`IsolationForest`, `StandardScaler`)
* **Topological Graph Engineering:** NetworkX
* **Interactive Visualization UI:** Streamlit, Plotly Express

---

## Directory Structure

```text
├── src/
│   ├── data_generator.py      # Simulates production ledger traffic with synthetic anomalies
│   ├── anomaly_engine.py      # Multi-dimensional Isolation Forest model pipeline
│   ├── network_analyser.py    # Topological graph mapping and component extraction
│   └── app.py                 # Streamlit multi-page dashboard interface
├── requirements.txt           # Production environment dependencies
└── README.md                  # Project documentation
