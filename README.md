# Structural-Health-Monitoring
Structural Health Monitoring GUI
This project is a Python-based GUI application for Structural Health Monitoring using machine learning. It allows users to load structural data from a CSV file, train a machine learning model, and evaluate its performance.
Features
Load structural health data (CSV format)
Automatically compute engineered features
Train a Random Forest model to detect anomalies
Evaluate model performance with a classification report and confusion matrix
GUI built with tkinter for ease of use
Requirements
Install dependencies using pip:
pip install pandas numpy scikit-learn matplotlib joblib
Usage
1. Run the script:
python structural_health_monitor_gui.py
2. In the GUI:
Click Load CSV Data to select and preview a dataset.
Click Train Model to train a Random Forest model.
Click Evaluate Model to display model metrics and a confusion matrix.
Input Data Format
Your CSV file should contain the following columns:
Vibration
Stress
Temperature
Label (Target column with class labels, e.g., Normal or Anomaly)
Feature Engineering
The application automatically generates these additional features:
Vib_Stress_Ratio = Vibration / Stress
Temp_Stress_Product = Temperature * Stress
Vib_Temp_Sum = Vibration + Temperature
Model
Algorithm: Random Forest Classifier
Scaler: StandardScaler
Trained model and scaler are saved as rf_gui_model.pkl and scaler_gui.pkl.
Output
Console-like text output in the GUI for data preview, training accuracy, and evaluation report
Matplotlib plot of confusion matrix
License
This project is for educational purposes.
Let me know if you’d like to add instructions for packaging or converting to an .exe.
