# team-candy-corn-sp25
# 🌱 Crop Recommendation System

## 📖 Project Overview
This project provides a **crop recommendation system** based on environmental factors such as **temperature, humidity, rainfall, soil pH, and nutrient levels (Nitrogen, Phosphorus, and Potassium).** Using data analysis and machine learning, the system predicts the most suitable crop for specific soil and climate conditions.

---

## 🧠 Machine Learning Approach

We trained a classification model to predict the **most suitable crops** based on input features. Key components:

- **Model**: Random Forest Classifier (scikit-learn)
- **Training Data**: Labeled dataset of historical soil + climate conditions and successful crops
- **Features**: N, P, K levels, pH, soil texture, temperature, humidity, wind speed, solar radiation, etc.
- **Output**: Top 3 crops based on probability ranking from the model

## 📊 Features

- Top 3 crop prediction for each land sample
- Interactive geospatial visualization using Plotly (color-coded by Top 1 crop)
- Python Flask backend for web-based crop recommendation

## 📁 Files

- `predict_top3_env_soil.py`: ML pipeline for training and prediction
- `crop_recommender_flask.py`: Flask app for user interface/API
- `最终整合推荐结果Top3.xlsx`: Final dataset with prediction results

## 🌍 Data Visualization

Interactive map shows predicted Top1 crop per location:
- Each point represents a land sample
- Color-coded by Top1 recommended crop
- Hover to see location and crop details

## 🚀 How to Run

1. Install dependencies:
   ```bash
   pip install pandas plotly flask scikit-learn

# crop-recommendation-system
