# 🎮 Video Game Recommender System (ALS Matrix Factorization)

This project implements a **Video Game Recommender System** using **Alternating Least Squares (ALS)** for collaborative filtering. It is based on the [Steam-200K dataset](https://www.kaggle.com/datasets/tamber/steam-video-games), which includes user-game interaction data such as playtime. The system generates personalized game recommendations and evaluates performance using **RMSE** and **MAE**.

---

## 🚀 Features
- **Data Preprocessing**:
  - Filter only `play` actions.
  - Apply `log1p` transformation to normalize playtime.
  - Map user and game IDs to numerical indices.

- **ALS Matrix Factorization**:
  - Factorizes the user-item interaction matrix into user and game latent factors.
  - Implements ALS from scratch (no third-party recommendation libraries).
  - Supports hyperparameter tuning with grid search.

- **Evaluation**:
  - Calculates **RMSE (Root Mean Square Error)** and **MAE (Mean Absolute Error)** on the test set.
  - Handles **cold-start** analysis for unseen users/games.

- **Recommendations**:
  - Generates top-N recommendations for a given user.
  - Filters out already played games.

---

## 🗂 Project Structure
