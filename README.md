# 🏠 House Price Prediction

Predicting Boston housing prices using supervised machine learning.  
📖 [Read the full tutorial on Medium](https://vrushalitandel1.medium.com/housing-price-prediction-step-by-step-implementation-of-machine-learning-project-9939e6c7c59e)

## 📊 Dataset
- Source: UCI Boston Housing Dataset
- 506 records, 14 features (crime rate, rooms, tax rate, etc.)

## 🔬 Approach
1. **Exploratory Data Analysis** — correlation matrix, scatter plots
2. **Feature Engineering** — created TAXRM (TAX/RM) attribute
3. **Data Preparation** — StratifiedShuffleSplit (80/20), SimpleImputer, StandardScaler
4. **Model Comparison:**

| Model | Mean RMSE | Std Dev |
|-------|-----------|---------|
| Decision Tree | 4.19 | 0.85 |
| Linear Regression | 4.22 | 0.75 |
| **Random Forest** ✅ | **3.49** | **0.76** |

5. **Evaluation** — K-Fold Cross Validation (N=10), final test RMSE: **3.22**

## 🛠️ Tech Stack
- Python 3
- pandas, numpy
- scikit-learn (RandomForestRegressor, Pipeline, SimpleImputer, StandardScaler)
- matplotlib
- joblib (model persistence)

## 🚀 How to Run
```bash
git clone https://github.com/VrushaliTandel/house-price-prediction.git
cd house-price-prediction
pip install -r requirements.txt
jupyter notebook house_price_prediction.ipynb
```

## 📁 Project Structure
house-price-prediction/
├── house_price_prediction.ipynb   # Main notebook
├── data.csv                       # Dataset
├── Dragon.joblib                  # Saved model
├── requirements.txt
└── README.md
