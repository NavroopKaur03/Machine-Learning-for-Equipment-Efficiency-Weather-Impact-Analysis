## 🚛 Machine Learning for Equipment Efficiency & Weather Impact Analysis

Client: Innoflow Energy Corp.
Note: Due to client confidentiality, project files are not publicly available.

## 📌 Project Summary
This project applies machine learning to address two key operational challenges at Innoflow's KORIKI and SAND OCEAN substations:

- Predicting fuel delivery delays influenced by extreme weather.

- Estimating equipment failure risks using usage patterns and operational metadata.

The ultimate goal is to enhance scheduling, reduce downtime, and support proactive maintenance decisions through predictive analytics and weather-integrated forecasting.

## 🎯 Project Goals
- 📍 Predict if a fuel delivery will exceed the long-duration threshold of 365 minutes.

- ⚙️ Classify equipment as “at-risk” based on operational history and usage trends.

- 🌡️ Discover how weather conditions correlate with delays and failures.

- 📈 Deliver insights to aid smart scheduling and maintenance strategies.

## 🧠 ML Models & Methodology
## 1️⃣ Fuel Delivery Delay Prediction
**Objective:** Classify deliveries as "long-running" or "on-time".
**Features Used:**
- Volume delivered
- Air temperature
- Time-based features: Hour, Day of Week, Weekend

**Feature Engineering:**
- Created delay labels based on average delivery duration
- Extracted time and weather patterns

**Model:** Random Forest Classifier

**Accuracy:** 97.28%

**Key Insights:**
- Delays are most common in early morning hours and sub-zero temperatures.

- Best delivery performance occurs midday in moderate weather (12°C–20°C).

## 2️⃣ Equipment Failure Risk Assessment
**Objective:** Predict failure-prone equipment based on status logs (DECOMM, OUTS).

**Features Used:**
- Equipment make & model

- Total fuel dispensed

- Days since last use

- Usage frequency

**Engineering:**

- Aggregated historical usage data

- Labeled failures and balanced dataset with SMOTE

**Model:** Random Forest (with SMOTE)

**Accuracy:** 93%

**Key Insights:**

- Emulsion Chargers had the highest failure rates.

- Light Vehicles had moderate failure risk but dominated the inventory (n=254).

## 📊 Data Visualization Highlights
- Delay trends spike in winter and during severe cold.

- Failure risk patterns vary by equipment type and usage behavior.

- Higher delivery volumes and warmer temperatures reduce delay probabilities.

## 🔎 Responsible AI & Ethics
✅ Fairness: Models validated to prevent geographic or seasonal bias.

✅ Transparency: Feature importance scores were shared with stakeholders.

✅ Privacy: Only anonymized environmental and operational data was used—no personal information involved.

## 🧰 Tools & Tech Stack
- Programming: Python

- Libraries: pandas, scikit-learn, matplotlib, seaborn

- Techniques: Random Forest, SMOTE (class balancing), feature engineering

- Platform: Jupyter Notebook

## 🔒 Note on Data Access
Due to client confidentiality policies, source code and datasets from this project are not included in the repository.
