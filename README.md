# 24MBMA23_AnkitSingh_Capstone
Capstone MBA project: agriculture trends, crop prices, market and sentiment prediction using big data.

# 🌾 Big Data Applications in Modern Agriculture

**Author:** Ankit Singh (24MBMA23)
**Course:** MBA - Big Data Analytics
**Institution:** University of Hyderabad
**Project Type:** Capstone

---

## 📘 Project Overview

This project leverages **Big Data Analytics** to address real-world challenges in **Indian agriculture**.
Using **PySpark** and **Databricks**, the system automates **data ingestion, transformation, model training**, and **alert generation** to deliver actionable insights for **farmers** and **policymakers**.

### 🎯 Objectives

* Analyze social media and digital data for real-time agricultural trends
* Predict market prices, farmer sentiment, pest outbreaks, and demand
* Generate regional alerts and recommendations for decision-making

---

## 🚜 Use Cases

### 1. Pest and Disease Warning for Farmers

* **Goal:** Detect spikes in pest-related keywords from farmer posts.
* **Output:** Region-wise alerts for pest outbreaks and preventive actions.

### 2. Real-Time Crop Price Prediction

* **Goal:** Forecast commodity prices by combining sentiment and engagement data.
* **Output:** Accurate, timely price estimates to guide farmers’ selling decisions.

### 3. Checking Farmers' Sentiments

* **Goal:** Analyze farmers’ emotions, opinions, and satisfaction levels.
* **Output:** Sentiment indices for policy-making and support planning.

### 4. Predicting Market Demand

* **Goal:** Use ML clustering to classify crops/regions by demand category.
* **Output:** Market demand clusters and trend forecasts for better crop planning.

### 5. Local Farming Alerts and Updates

* **Goal:** Automate regional notifications for threats, pricing, and market info.
* **Output:** Mobile alerts and dashboard insights for farmers and officials.

---

## 📊 Dataset

* **Source:** Social media, agricultural forums, and survey data
* **Format:** CSV (Structured, ~3,000+ records for pilot)

### Fields:

| Field                 | Description                 |
| --------------------- | --------------------------- |
| Region                | Geographic area             |
| Crop                  | Crop name                   |
| Emotion               | Sentiment score/category    |
| PostText              | Farmer’s message or comment |
| Date                  | Post or record timestamp    |
| Price, DemandIndex    | Market-related fields       |
| Temperature, Rainfall | Weather parameters          |

---

## ⚙️ Implementation Methodology

### Platform:

* **Databricks** (PySpark Notebooks/Workflows)

### 🔁 Pipeline Steps:

1. **Ingestion & Validation** – Load CSV, clean data, handle missing values
2. **Transformation** – Normalize fields, compute sentiment (positive/negative/neutral)
3. **Feature Engineering** – Create pest flags, aggregate regional data, rolling metrics
4. **Model Training** –

   * *Random Forest Regression* → Crop price prediction
   * *K-Means Clustering* → Demand segmentation
5. **Alert Generation** – Trigger alerts based on thresholds (z-score, sentiment, demand)

### 🧰 Technologies Used

* **PySpark**, **Spark MLlib**
* **Databricks** (or local Spark setup)
* **Python**, **Matplotlib**, **Seaborn** (for visualization)

---

## 📈 Results & Outputs

| Use Case                 | Visualization    | Insight                                           |
| ------------------------ | ---------------- | ------------------------------------------------- |
| Pest & Disease Detection | Line chart       | Detects spikes in pest mentions; alerts generated |
| Price Prediction         | Time-series plot | Predicts market prices accurately                 |
| Sentiment Monitoring     | Bar chart        | Shows region-wise farmer sentiment                |
| Market Demand Clusters   | Scatterplot      | Helps crop planning and policy                    |
| Alert Recommendations    | Dashboard/Table  | Displays active alerts and suggested actions      |

---

## 💬 Discussion

* Positive farmer sentiment often precedes **market price rises**.
* Negative sentiment correlates with **pest problems** and **demand drops**.
* Automated alerts enable **early farmer response**, improving yield and reducing loss.
* The end-to-end pipeline is **scalable** and adaptable for larger datasets or regions.

---

## ⚠️ Limitations

* Static dataset (no real-time streaming yet).
* Sentiment analysis limited to **English text**.
* Models require **periodic retraining** as data evolves.

---

## 🚀 Future Enhancements

* Integrate **live social media APIs** (Twitter/Facebook).
* Add **real-time dashboards** using Power BI or Streamlit.
* Deploy as a **REST API** for government or NGO use.
* Incorporate **IoT and weather station data** for higher precision.

---

## 🧩 How to Run

1. **Clone this repository**

   ```bash
   git clone https://github.com/yourusername/BigData-Agriculture.git
   cd BigData-Agriculture
   ```
2. **Import CSV dataset(s)** into Databricks or PySpark environment
3. **Run notebooks in sequence:**

   * `01_ingestion.ipynb`
   * `02_transformation.ipynb`
   * `03_feature_engineering.ipynb`
   * `04_model_training.ipynb`
   * `05_alert_generation.ipynb`
4. **View results** in dashboards, charts, and output tables

---

## 📜 License

**Academic and Educational Use Only**
© 2025 Ankit Singh, University of Hyderabad

