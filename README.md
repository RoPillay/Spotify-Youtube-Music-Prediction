# Spotify–YouTube Music Prediction

This project was developed as part of a **STA160 Data Science Capstone at the University of California, Davis**.

The goal of this project was to analyze cross-platform music data from **Spotify and YouTube** to understand the factors that drive **song popularity and marketability**. Using audio features and audience engagement metrics, we developed machine learning models capable of predicting song success and exploring patterns in music performance.

---

## Project Overview

We constructed a dataset of **5,700+ songs** by collecting and integrating data from:

- Spotify Web API
- YouTube Data API
- Audio feature extraction using `librosa`

The dataset combines:

**Audio features**
- energy
- danceability
- tempo
- valence
- loudness
- acousticness
- duration

**Engagement metrics**
- YouTube views
- likes
- comments
- Spotify popularity

This allows us to analyze both **musical characteristics and listener behavior**.

---

## Machine Learning Models

We evaluated several models, including:

- Random Forest
- CNN (audio-based model)
- XGBoost
- CatBoost
- LightGBM
- Bayesian Optimization

The **final XGBoost model** performed best.

| Target | R² | MAE |
|------|------|------|
| Popularity Prediction | 0.656 | 5.02 |
| Marketability Prediction | 0.698 | 2.02 |

These results show that **listener engagement metrics are the strongest predictors of song success**, while audio features provide additional signal.

---

## Interactive Dashboard

We built an **interactive dashboard using Dash and Plotly** that allows users to:

- explore audio feature distributions
- analyze engagement trends
- view predicted popularity and marketability scores
- upload songs for prediction
- search artists and tracks

⚠️ **Note:**  
The dashboard is not currently deployed because hosting required a paid cloud service due to the large machine learning models and audio embeddings used. Screenshots and full documentation of the dashboard are available in the final report.

---

