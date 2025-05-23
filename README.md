# 🌽 Crop Recommendation System

This machine learning project provides crop recommendations based on environmental and soil characteristics across U.S. regions. Built as part of the UIUC Data Science Club, it helps farmers choose the most suitable crops using advanced modeling and clustering techniques.

## 🚀 Project Objective

To analyze soil nutrient levels and climatic data (rainfall, temperature, humidity) and recommend optimal crops for a given region, supporting data-driven decisions in agriculture.

## 🧠 Models & Techniques

- Random Forest
- XGBoost (main model)
- K-Nearest Neighbors (KNN)
- Multi-Layer Perceptron (MLP)
- Support Vector Machine (SVM)
- Unsupervised clustering (K-Means) for crop grouping

## 📁 Project Structure

├── data/ # All datasets (raw + processed)
├── models/ # Trained models (.pkl files)
├── notebooks/ # Exploratory analysis and model training
│ ├── Crop_prediction.ipynb
│ ├── MLcomparison.ipynb
│ └── Crop cluster.ipynb
├── README.md


## 📊 Key Results

- XGBoost achieved highest crop prediction accuracy.
- Clustered crops into market-tuned categories based on shared growing conditions.
- Built region-specific crop recommendations integrating environmental layers.

## 🔧 Tech Stack

- Python (Pandas, NumPy, Matplotlib)
- Scikit-learn, XGBoost, Seaborn
- Jupyter Notebook
- Git, GitHub

## 🤝 Contributors

- **Yunya Lin** – [LinkedIn](https://www.linkedin.com/in/yoyo-lin-631889299/)  
- **Tianqi Zhang**  
- **Sujia Guo**

> This project was developed collaboratively as part of the UIUC Data Science Club (IDSC) in Spring 2025.

## 📜 License

This project is open-source and available for academic and educational use.
