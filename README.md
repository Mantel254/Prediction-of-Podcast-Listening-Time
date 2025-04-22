# 🎧 Prediction of Podcast Listening Time

This project is developed for the Kaggle competition:  
👉 [Playground Series - Season 5, Episode 4](https://www.kaggle.com/competitions/playground-series-s5e4/overview)

The objective is to predict how long users will listen to podcast episodes using historical data and metadata. This helps in understanding user preferences and improving recommendation systems.
Attained root mean is 12.61560

## 📁 Repository Contents

- `submision5.ipynb`: Main notebook that includes data loading, exploration, preprocessing, feature engineering, model training, and prediction generation.
- `train.csv`, `test.csv`: Datasets provided by the competition.
- `sample_submission.csv`: Format to be used for submitting predictions on Kaggle.

## 🧪 Competition Objective

You're given:
- Metadata about podcasts and users
- User listening behavior
- Podcast attributes like duration, release date, and playback speed

**Goal:** Predict the `listening_duration` for the test dataset.

## 🧠 Approach

1. **Data Preprocessing**
   - Handling nulls and outliers
   - Parsing dates and numeric conversions

2. **Feature Engineering**
   - Time-based features (day of week, hour, etc.)
   - Derived features such as adjusted speed metrics

3. **Model Training**
   - Gradient Boosting with LightGBM
   - Evaluation using RMSE (Root Mean Squared Error)
   - Cross-validation for robustness

4. **Submission**
   - Generating a submission file in `.csv` format

## 📦 Requirements

Install necessary libraries with:

```bash
pip install pandas numpy lightgbm scikit-learn matplotlib seaborn
