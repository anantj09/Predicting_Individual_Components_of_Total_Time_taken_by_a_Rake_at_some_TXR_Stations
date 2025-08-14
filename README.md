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

## 🛠️ Methodology
The project workflow was structured as follows:
1. Data Preprocessing: The initial dataset containing rake movement and examination details for multiple stations was rigorously cleaned and prepared for analysis.
2. Feature Engineering: New, informative features were engineered to capture the dynamic nature of station operations. The introduction of congestion-based metrics was crucial for enhancing model performance.
3. Model Training & Evaluation: Several regression models were trained on individual station datasets to predict the target durations. Model performance was meticulously evaluated to identify the most effective algorithms.

## 🤖 Models Implemented
A suite of powerful regression models was employed to tackle the prediction tasks:
- Random Forest Regressor
- Support Vector Regressor (SVR)
- K-Nearest Neighbors (KNN) Regressor
- XGBoost Regressor
- LightGBM Regressor

## 📊 Results & Performance
The integration of engineered features, especially the congestion metrics, led to a significant improvement in model performance. Key observations from the DDU station case study include:
- Performance Boost: R^2 (R-squared) values saw a substantial increase, moving from low or even negative values to strong positive scores post-feature engineering.
- Top Performers: LightGBM and XGBoost consistently delivered the best performance across most prediction targets.
- Predictability: The Placement to Release duration was the most predictable phase, likely due to its more structured nature.
- Challenge Area: The Release to Departure phase proved to be the most challenging to predict, highlighting it as an area for further operational analysis.

## 💡 Conclusion
The models developed in this project provide valuable, data-driven insights into dynamic station bottlenecks. They serve as a robust foundation for optimizing railway operations and improving asset turnaround. The challenging predictability of the "Release to Departure" phase suggests that external factors or more complex operational dependencies may be at play, marking a clear direction for future research.

## 🙏 Acknowledgements
This project was developed as part of an internship at the Centre for Railway Information Systems (CRIS). The work was carried out under the valuable guidance and mentorship provided by the team at CRIS. Their support was instrumental in the successful completion of this analysis.

## 📁 Dataset
The dataset used for this project is included in this GitHub repository. It contains detailed records of rake movements and examination timings at the relevant TXR stations.

## ⚙️ Installation
1. Clone the repository to your local machine:

        git clone https://github.com/anantj09/Predicting_Individual_Components_of_Total_Time_taken_by_a_Rake_at_some_TXR_Stations.git

2. Install the required libraries using the requirements.txt file:
        pip install -r requirements.txt

The required libraries are: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, and shap.

## 🚀 Usage
To run the analysis and train the models, please follow these steps in order:
1. Run Initial Setup: First, open and run the txr_start.ipynb notebook from start to finish. This file likely handles the initial data loading, cleaning, and preprocessing steps required for all stations.
2. Run Station-Specific Analysis: After completing the first step, you can run any of the station-specific notebooks (e.g., txr_ddu.ipynb, txr_stationname.ipynb) to see the individual modeling and results for that particular station.
