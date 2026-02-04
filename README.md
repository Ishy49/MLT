🚆 Smart Train Delay Mitigation System

📌 Project Overview

The Smart Train Delay Mitigation System is a machine learning–based project designed to analyze railway delay patterns and provide proactive mitigation suggestions.
Instead of only predicting delays, the system classifies delay risk levels and recommends actions that help reduce the impact on passengers and railway operations.

This project demonstrates how historical railway delay data can be transformed into an intelligent decision-support system.

🎯 Objectives

Perform preprocessing and feature engineering on railway delay datasets.

Build a machine learning model to predict delay risk levels.

Generate mitigation suggestions based on predicted risk.

Demonstrate a scalable architecture that can integrate with real-time railway data.

📊 Dataset

Dataset used: etrain_delays.csv

Features

train_number – Unique train identifier

station_code – Station code

station_name – Station name

avg_delay_min – Average delay in minutes

pct_right_time – Percentage of trains on time

pct_slight_delay – Percentage of slight delays

pct_significant_delay – Percentage of significant delays

total_records – Number of observations

day_of_week – Engineered feature

month – Engineered feature

season – Feature created during preprocessing

Dataset size: 1900+ rows

⚙️ Project Workflow

1️⃣ Data Preprocessing

Cleaned column names

Handled missing values

Converted data types

Added engineered features:

day_of_week

month

season

Applied Label Encoding on categorical variables

Applied StandardScaler to normalize numerical features

2️⃣ Risk Level Creation

Delay risk categories were created using avg_delay_min:

Low Risk – Minimal delays

Medium Risk – Moderate delays

High Risk – Significant delays

This transformed the problem into a classification task.

3️⃣ Model Training

Model used:

Random Forest Classifier

Steps:

Train-test split (80/20)

Model training using selected features

Performance evaluation using accuracy metrics

4️⃣ Mitigation Engine

The mitigation system generates recommendations based on predicted risk:

Risk Level	Mitigation Suggestion
Low	Normal operation
Medium	Monitor train closely
High	Notify passengers early

This makes the system proactive rather than reactive.

🧠 Technologies Used

Python

Google Colab

Pandas

NumPy

Scikit-learn

📂 Project Structure
Smart-Train-Delay-Mitigation-System/
│
├── etrain_delays.csv
├── cleaned_etrain_delays.csv
├── notebook.ipynb
├── README.md
▶️ How to Run the Project

Open the notebook in Google Colab.

Upload the dataset file.

Run preprocessing cells.

Train the model.

Generate risk predictions and mitigation outputs.

📈 Future Improvements

Integrate live railway API data for real-time predictions.

Add visualization dashboards.

Deploy using a web interface.

Improve model accuracy using advanced ensemble methods.

🎓 Academic Use

This project was developed as a B.Tech AI & Data Science Mini Project to demonstrate applied machine learning concepts in transportation analytics.

📜 License

This project is intended for educational purposes.
