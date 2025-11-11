# 24MBMA23_AnkitSingh_Capstone
Capstone MBA project: agriculture trends, crop prices, market &amp; sentiment prediction using big data.
Big Data Applications in Modern Agriculture
Author: Ankit Singh (24MBMA23)
Course: MBA - Big Data Analytics
Institution: University of Hyderabad
Project Type: Capstone

Project Overview
This project leverages Big Data Analytics to solve practical problems in Indian agriculture. Using PySpark and Databricks, the solution automates data ingestion, transformation, model training, and alert generation to deliver actionable insights for farmers and policymakers. The main objectives are:

Analyze social media and digital data for real-time agricultural trends

Predict market prices, farmer sentiment, pest outbreaks, and demand

Generate regional alerts and recommendations to inform decision-making

Use Cases
Pest and Disease Warning for Farmers:
Detect spikes in pest-related keywords using text analysis on farmer posts.
Output: Region-wise alerts for pest outbreaks and preventive actions.

Real-Time Crop Price Prediction:
Forecast commodity prices by combining sentiment scores and engagement data.
Output: Accurate, timely price estimates to guide selling decisions.

Checking Farmers' Sentiments:
Monitor and analyze farmers' emotions, opinions, and feedback to track satisfaction.
Output: Sentiment indices used for policy and support planning.

Predicting Market Demand:
Use ML clustering to classify regions/crops into demand categories.
Output: Market demand clusters and trend forecasts for crop planning.

Local Farming Alerts and Updates:
Automate region-wise notifications for threats, pricing, and market recommendations.
Output: Mobile alerts and dashboard insights for farmers and officials.

Dataset
Source: Social media, agricultural forums, and survey data

Format: CSV (Structured, 3,000+ records for pilot)

Fields:

Region

Crop

Emotion (sentiment)

PostText

Date

Price, DemandIndex

Temperature, Rainfall

Implementation Methodology
Platform: Databricks (PySpark notebooks/workflows)

Pipeline Steps:

Ingestion & Validation: Load and clean CSV, handle missing values

Transformation: Normalize fields, compute sentiment scores (positive/negative/neutral)

Feature Engineering: Create flags for pests, aggregate region-wise data, rolling metrics

Model Training: Apply Random Forest for regression (price), K-Means for segmentation (demand)

Alert Generation: Trigger notifications based on thresholds (z-score, sentiment, demand)

Technologies Used:

PySpark, Spark MLlib

Databricks (or local Spark)

Python, Matplotlib, Seaborn (visualization)

Results & Output
Pest and Disease Detection:
Line chart shows spikes in pest mentions; dashboard triggers alerts for control measures

Price Prediction:
Time series plots of predicted vs. actual prices; reliable estimation performance

Sentiment Monitoring:
Bar charts of region-wise farmer sentiment; identifies areas needing support

Market Demand Clusters:
Scatterplot of demand categories; helps farmers and authorities plan crops

Alert Recommendations:
Table/dashboard with active alerts; suggested actions and updates

Discussion
Positive sentiment trends precede market price rises; negative sentiment links to pest issues and demand drops

Automated alerts help farmers act earlier, increase yield, and reduce losses

The end-to-end pipeline is scalable and easy to adapt for more data or regions

Limitations
Dataset is static; real-time streaming (API integration) is a future step

Sentiment analysis currently English-only; needs for multi-language support

Models need retraining as data evolves for best accuracy

Future Enhancements
Integrate live social media feeds (Twitter/Facebook API)

Add dashboard for real-time visualization (Power BI, Streamlit)

Deploy as a REST API for government/NGO usage

Incorporate IoT and weather station data for precision insights

How to Run
Clone this repository

Import CSV dataset(s) into Databricks or your PySpark environment

Run notebooks in sequence: ingestion → transformation → feature engineering → model training → alert generation

View results in output dashboards, charts, and tables

License
Academic and educational use only.

