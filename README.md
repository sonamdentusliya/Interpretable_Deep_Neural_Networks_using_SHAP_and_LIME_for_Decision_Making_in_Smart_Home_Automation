# 🏠 Interpretable Deep Neural Networks using SHAP and LIME for Decision Making in Smart Home Automation
# 📌 Project Overview

This project presents an interpretable deep learning framework for smart home automation using SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-Agnostic Explanations).

A virtual smart home environment was designed using Tinkercad, where sensor readings were simulated and collected. These readings were stored in a CSV dataset and used to train Deep Neural Network (DNN) models for predicting smart home device states such as:

🚪 Door Status (Open / Closed)

🔔 Buzzer Status (ON / OFF)

💡 Bulb Status (ON / OFF)

🚶 Motion Detection (Motion / No Motion)

The project not only builds predictive models but also explains model decisions using Explainable AI techniques.

# 🏗 Smart Home Simulation (Tinkercad)

The virtual smart home was designed and simulated using Tinkercad.

🔗 Tinkercad Smart Room Design:
https://www.tinkercad.com/things/hRPzXGGZ5VF-smart-room?sharecode=uulnG78UKgjD3bmNm0H8817tBYx4l82i0Q8qGCEPAW8

Sensors Used:

🌞 LDR Sensor (Light intensity)

🚶 PIR Motion Sensor

🛢 Gas Sensor

📏 Ultrasonic Distance Sensor

The readings generated during simulation were manually recorded into a CSV file: smart_home_data_125_samples.csv

# 🧠 Technologies Used

Python

TensorFlow / Keras

Scikit-learn

SHAP

LIME

Pandas & NumPy

Matplotlib & Seaborn

# 📊 Machine Learning Workflow
1️⃣ Data Collection

-> Sensor values collected from Tinkercad simulation

-> Stored in CSV format

-> 125 samples used for training and testing

2️⃣ Data Preprocessing

-> Categorical encoding (ON/OFF → 0/1)

-> Feature selection:

      LDR Value

      Gas Value

      Distance

Motion Status (when applicable)

3️⃣ Model Architecture

A Deep Neural Network (DNN) was built using TensorFlow:

        Input Layer
            ↓
       Dense Layer (ReLU)
            ↓
      Dense Layer (ReLU)
            ↓
    Output Layer (Sigmoid - Binary Classification)

Loss Function: Binary Crossentropy

Optimizer: Adam

Evaluation Metrics: Accuracy, Confusion Matrix, Classification Report

# 🔍 Explainable AI Integration

To make the model interpretable and trustworthy:

✅ SHAP (Global + Local Interpretability)

-> Feature importance visualization

-> Contribution of each sensor to predictions

SHAP summary and bar plots

✅ LIME (Local Interpretability)

-> Explains individual predictions

-> Shows which sensor values influenced a specific decision

-> Model-agnostic explanation

# 📈 Output Visualizations

Confusion Matrix

Classification Report

SHAP Summary Plots

SHAP Feature Importance Bar Plots

LIME Instance-level Explanation
