# Predicting_Individual_Components_of_Total_Time_taken_by_a_Rake_at_some_TXR_Stations

## 📜 Overview
This project focuses on predicting the various components of rake turnaround time at several Train Examination (TXR) stations using machine learning. By analyzing a dataset of rake movements, we developed predictive models to forecast critical time intervals, aiming to optimize railway asset utilization and improve operational efficiency. The core of this project lies in extensive feature engineering, particularly the creation of novel congestion metrics to quantify station occupancy in real-time.

While the methodology is applicable across multiple stations, the initial analysis on the DDU station serves as a key case study.

## ✨ Key Features

- Multi-Station Analysis: Models are developed for various TXR stations to provide a scalable solution.
- Component Prediction: Utilizes machine learning to forecast key operational durations:
    - Arrival to Placement
    - Placement to Release
    - Release to Departure
- Advanced Feature Engineering: Goes beyond standard features by creating:
- Cyclical Time Components: Encodes time-of-day and day-of-week patterns.
- Rake Type Encodings: Differentiates between various types of rakes.
- Congestion Metrics: A novel approach to measure real-time station occupancy and bottlenecks.
