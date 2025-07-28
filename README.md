# 🏏 IPL Win Probability Predictor

A machine learning-based web application that predicts the win probability of IPL teams in real-time using historical match and ball-by-ball data.

## 📌 Overview

This project uses historical IPL data to predict second-innings win probabilities based on real-time match conditions. It combines logistic regression with feature engineering on datasets like `matches.csv` and `deliveries.csv`.

## ⚙️ Features

- ✅ Trained logistic regression model with ~85% accuracy
- 📊 Feature engineering using:
  - Current score
  - Wickets fallen
  - Balls left
  - Target and required run rate
- 🧹 Data cleaning: removed D/L method matches, renamed teams
- 💾 Model serialized (`pipe.pkl`) for easy deployment
- 🖥️ Simple frontend (PyCharm) for live inputs and win probability output

## 🗃️ Dataset

- `matches.csv`: Summary of each IPL match  
- `deliveries.csv`: Ball-by-ball data for every game  
Source: [Kaggle IPL Dataset](https://www.kaggle.com/datasets)

## 🧠 Model Training

- Input features:
  - Runs left
  - Balls left
  - Wickets in hand
  - Current and required run rate
  - Team strengths
- Algorithm: Logistic Regression
- Accuracy: ~85%

## 🚀 Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/AkshatSarin2004/IPL-Win-Probability-Predictor.git
   cd repo
2. Install dependencies:
   pip install -r requirements.txt
   
3. Run the predictor:
    python app.py
   
🖼️ UI Preview
Enter match stats like runs, wickets, balls left, and see real-time win probability for both teams. 

📁 File Structure
repo/
├── data/
│   ├── matches.csv
│   └── deliveries.csv
├── pipe.pkl
├── predictor.py
├── app.py
├── README.md
└── requirements.txt

   
