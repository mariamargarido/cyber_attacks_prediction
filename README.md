# Cyber_Attacks_Prediction
Cyber Attack Data Prediction (Big Data Project)

📌 Project Overview

This project focuses on analyzing and predicting the amount of bytes transferred during cyber attacks using the UNSW-NB15 dataset. Leveraging Big Data technologies and Machine Learning, the goal was to build regression models capable of estimating the variable dbytes, which represents the data volume received by attackers.

The project was developed within the Big Data course of the Master’s in Data Analysis and Decision Support Systems (MADSAD) at Coimbra Business School – ISCAC.

⚙️ Technologies Used

  o Apache Spark (PySpark) – distributed data processing
  
  o Spark MLlib – implementation of regression models
  
  o Pandas – data manipulation and preprocessing
  
  o Matplotlib & Seaborn – data visualization

📊 Methodology

1. Data preparation
2. Import and merge UNSW-NB15 CSV files
3. Handle missing values and anomalies
4. Normalize numerical features (StandardScaler)
5. Encode categorical features (StringIndexer + OneHotEncoder)
6. Filtered dataset to include only malicious traffic
7. Feature selection
8. Pearson correlation (numerical variables)
9. Chi-Square test (categorical variables)
10. Selected top 15 most relevant features
11. Modeling
12. Implemented and compared three regression models:
13. Linear Regression (RL)
14. Random Forest Regressor (RFR)
15. Gradient Boosting Trees (GBT)
16. Evaluation metrics: RMSE, MAE, R²

Results

Linear Regression outperformed all models

Achieved R² = 0.9973 and RMSE ≈ 5404.40

Trained in just 106s, much faster than RFR and GBT

Demonstrated that the relationship between features and dbytes is predominantly linear

🚀 Key Findings

  - Simple linear models can be highly effective for cybersecurity tasks involving traffic volume prediction.
  
  - Feature engineering and proper data preparation have a critical impact on model performance.
  
  - Results suggest that predictive analytics can support real-time attack detection and mitigation.

📂 Dataset

UNSW-NB15: a benchmark dataset for network traffic analysis and cybersecurity research.
Contains both normal and malicious traffic records with attributes such as duration, packets, protocols, and byte counts.
