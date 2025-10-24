🧠 Uber Trip Analysis – Machine Learning Project
📋 Project Overview

This project focuses on analyzing Uber trip data to identify patterns, peak demand times, and build a predictive model for estimating future trip demand.
The analysis involves data preprocessing, EDA, feature engineering, model training, evaluation, and visualization using Python.

🧰 Tech Stack & Tools

Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

Algorithm: Random Forest Regressor

IDE: Jupyter Notebook / VS Code

Dataset: Uber-Jan-Feb-FOIL.csv

📊 Dataset Description

The dataset contains Uber pickup information for January and February 2015, including:

Column Name	Description
Date/Time / Pickup_date	Timestamp of the pickup
Lat	Latitude of the pickup
Lon	Longitude of the pickup
Base / Dispatching_base_num	TLC base company code
locationID	Pickup zone ID
Trips	Number of trips (aggregated or derived)
⚙️ Implementation Steps
1️⃣ Data Preprocessing

Loaded dataset and converted Date/Time to datetime format.

Extracted Hour, Day, Month, and DayOfWeek.

Handled missing values and created dummy variables for Base codes.

2️⃣ Exploratory Data Analysis (EDA)

Visualizations created to understand trip behavior:

Trips per hour and day of the week

Trips per month

Heatmap (Day vs Hour) showing time-based demand

Base company trip distribution

Correlation matrix for numerical relationships

3️⃣ Feature Engineering

Added derived time features and categorical encodings.

Selected key features for model training: Hour, Day, DayOfWeek, Month, Lat, Lon.

4️⃣ Model Building

Used Random Forest Regressor to predict trip demand.

Split data into 70% training and 30% testing sets.

Trained and validated the model on extracted features.

5️⃣ Model Evaluation

Evaluated using:

Mean Squared Error (MSE)

R² Score

Visualized Actual vs Predicted Trips and Feature Importance.

📈 Results & Insights

Peak hours: 6 PM – 9 PM

Busiest days: Friday and Saturday

Top base company: B02512 (Unter)

Model Accuracy: R² ≈ 0.85

Conclusion: Random Forest effectively predicts Uber trip demand based on time and location.

🚀 Future Enhancements

Integrate XGBoost and Gradient Boosting for improved accuracy.

Add Geospatial visualization (Folium) for pickup hotspots.

Extend dataset to full-year analysis.

Deploy the model with Streamlit dashboard for real-time insights.

📚 References

Uber NYC TLC FOIL Data

Kaggle Uber Trip Analysis Dataset

scikit-learn, Pandas, Seaborn documentation
