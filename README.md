# Fraud Detection Project – Azure Databricks

This project demonstrates an end-to-end machine learning workflow for credit card fraud detection using **Azure Databricks**, **PySpark**, and **MLlib**.  
It includes both manual and automated pipelines for model training, evaluation, and retraining using **MLflow** and **Databricks Jobs**.

---

## Overview

This project contains two main notebooks:

1. **fraud_detection.ipynb**  
   - Data exploration and preprocessing  
   - Feature engineering and scaling  
   - Model training using Logistic Regression and Gradient Boosted Trees (GBT)  
   - Model evaluation using ROC-AUC, precision, recall, and confusion matrix  

2. **fraud_detection_pipeline.ipynb**  
   - Full pipeline automation  
   - Integration with MLflow for experiment tracking  
   - Designed for scheduled retraining using Databricks Jobs  

---

## Automation (Job Scheduling)

This project also demonstrates automation through **Azure Databricks Lakeflow Jobs**:
- Scheduling and monitoring pipeline execution  
- Automating model retraining  
- Managing experiment runs through MLflow  

---

## Tech Stack

- **Azure Databricks**
- **PySpark / Spark MLlib**
- **MLflow** for experiment tracking
- **Databricks Lakeflow Jobs** for scheduling and automation
- **Pandas**, **NumPy**, and **Matplotlib** for analysis and visualization

---

## Project Structure

```plaintext
fraud-detection-databricks-project/
│
├── notebooks/
│   ├── fraud_detection.ipynb
│   ├── fraud_detection_pipeline.ipynb
│
└── README.md
```

---
##  Dataset

The dataset used in this project is publicly available:
[Download from Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)

Due to size limitations, the dataset is not included in this repository.
------
## Learning Outcomes

```plaintext
• Understanding data preprocessing and feature engineering in Spark  
• Building scalable ML pipelines in Databricks  
• Automating model retraining with Databricks Jobs  
• Tracking experiments and metrics using MLflow  
• Applying machine learning techniques for fraud detection  
```

---

## Installation & Usage

```plaintext
1. Clone the Repository
   git clone https://github.com/Bahar15984/fraud-detection-databricks-project.git
   cd fraud-detection-databricks-project

2. Upload Notebooks to Databricks
   - Open your Azure Databricks workspace.
   - Navigate to: Workspace → Import → Notebook
   - Upload both notebooks:
       • fraud_detection.ipynb
       • fraud_detection_pipeline.ipynb

3. Set Up the Environment
   Ensure your cluster has the following libraries installed:
       pyspark
       mlflow
       pandas
       numpy
       matplotlib

   You can install them using:
       pip install pyspark mlflow pandas numpy matplotlib

4. Run the Notebooks
   - Run fraud_detection.ipynb first for preprocessing and model training.
   - Then run fraud_detection_pipeline.ipynb for automated retraining with MLflow & Lakeflow Jobs.

5. View Results
   - Go to MLflow → Experiments in Databricks to view tracked runs, metrics, and models.
   - Check Lakeflow Jobs for scheduled retraining automation.
```

---

## Author

```plaintext
Created by: Bahar Almasi  
Azure Databricks | PySpark | Machine Learning | MLOps
```

