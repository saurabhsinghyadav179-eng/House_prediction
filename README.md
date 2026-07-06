
# 🏠 House Price Prediction using Machine Learning

## 📌 Overview

This project builds and compares regression models to predict house prices based on features like median income, house age, average rooms, and location. It's designed to be beginner-friendly while covering a complete ML workflow — from raw data to a trained, evaluated model.

## ✨ Features

- 📊 Exploratory Data Analysis with distribution plots and a correlation heatmap
- 🧹 Clean, ready-to-run data pipeline (no manual dataset download needed)
- 🤖 Two trained models: **Linear Regression** and **Random Forest Regressor**
- 📈 Model evaluation using MAE, RMSE, and R² score
- 🔍 Feature importance visualization to explain predictions
- ☁️ Runs entirely in Google Colab — zero local setup required

## 🖼️ Preview

| Price Distribution | Correlation Heatmap | Feature Importance |
|:---:|:---:|:---:|
| Histogram of house prices | Heatmap of feature relationships | Bar chart of top predictive features |

*(Generated automatically when you run the notebook — screenshots can be added here after your first run.)*

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3 |
| Data Handling | pandas, NumPy |
| Visualization | matplotlib, seaborn |
| Machine Learning | scikit-learn |
| Environment | Google Colab / Jupyter Notebook |

## 📁 Project Structure

```
house-price-prediction/
├── House_Price_Prediction.ipynb   # Main notebook (EDA + models + evaluation)
└── README.md                      # Project documentation
```

## 🚀 Getting Started

### Run in Google Colab (recommended)
1. Click the **"Open in Colab"** badge above
2. Go to `Runtime → Run all`
3. That's it — the dataset loads automatically via scikit-learn, no downloads needed

### Run locally
```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
jupyter notebook House_Price_Prediction.ipynb
```

## 🧠 Methodology

1. **Load Data** — California Housing dataset via `sklearn.datasets.fetch_california_housing`
2. **Explore** — visualize price distribution, feature correlations, and income vs price trends
3. **Split Data** — 80/20 train-test split
4. **Train Models** — Linear Regression (baseline) and Random Forest Regressor (advanced)
5. **Evaluate** — compare models using MAE, RMSE, and R²
6. **Interpret** — visualize which features matter most for predicting price

## 📊 Results

| Model | MAE ↓ | RMSE ↓ | R² Score ↑ |
|---|:---:|:---:|:---:|
| Linear Regression | ~0.53 | ~0.75 | ~0.60 |
| **Random Forest** | **~0.33** | **~0.51** | **~0.80** |

> Random Forest consistently outperforms Linear Regression, capturing non-linear relationships in the data. *(Exact values may vary slightly by run/library version.)*

**Most influential feature:** `MedInc` (Median Income) — unsurprisingly, income level is the strongest predictor of house price.

## 🗺️ Roadmap

- [ ] Add Gradient Boosting / XGBoost for comparison
- [ ] Hyperparameter tuning with `GridSearchCV`
- [ ] Add cross-validation for more robust evaluation
- [ ] Deploy as an interactive web app (Streamlit/Flask)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m "Add YourFeature"`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request


