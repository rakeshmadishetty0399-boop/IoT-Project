 Energy Forecasting: Centralized vs Federated Learning

This repository contains the implementation and research logs for the project:

Comparing Federated and Centralized CNN–LSTM Attention for Uncertainty-Aware Appliance Energy Forecasting

---

 Project Overview
Smart homes generate large amounts of energy data through IoT devices.  
The aim of this project is to build a trustworthy forecasting system that can:  
- Predict appliance-level energy usage accurately  
- Preserve household privacy using Federated Learning  
- Provide uncertainty-aware forecasts to support risk-aware decision making  

We compare two training approaches:  
- Centralized Training → all data combined on a server  
- Federated Training → data stays local, only model updates are shared  

---

##  Repository Contents
- `EnergyForecasting.ipynb` → Jupyter Notebook with full implementation (data preprocessing, model, training, evaluation).  
- Research Log → submitted separately (for assessment).  
- Documentation of results and comparisons between centralized and federated setups.  

---

##  Model Design
- Hybrid CNN–GRU/LSTM with Attention
- Multi-task output:  
  - Regression for continuous energy consumption  
  - Classification for high-usage events  
- Uncertainty estimation: Monte Carlo Dropout  
- Evaluation Metrics: F1-score, Precision, Recall, Accuracy, MAE  

---

##  Dataset
The dataset used in this project is: **`PlegmaDataset_Clean.7z`** (~1.7 GB).  
Due to GitHub size limits, the dataset is hosted externally.  

## [Download Dataset Here]) #  https://drive.google.com/file/d/13OFIxp0PvgXRohJnfAnqh6qP6U506dXM/view?usp=drive_link  

After downloading, extract the archive and place it in your working directory before running the notebook.  

---

##  Running the Notebook
1. Download and extract the dataset.  
2. Open `EnergyForecasting.ipynb` in Jupyter Notebook or Google Colab.  
3. Update the dataset path in the notebook if needed.  
4. Run all cells to reproduce training, evaluation, and results.  

---

##  Key Results
- Centralized Training: F1 ≈ 0.92, Accuracy ≈ 0.88  
- Federated Training: F1 ≈ 0.91, Accuracy ≈ 0.90  
- Conclusion: Federated learning achieves near-centralized accuracy while preserving privacy.  

---

##  Author
- Rakesh Madishetty  
- Student ID: A00012185  
- Module: Research Log Submission  

---

