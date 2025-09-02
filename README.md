# 🚗 Second-Hand Car Price Prediction using Machine Learning

This project demonstrates a complete machine learning pipeline to predict the prices of second-hand cars using a mock dataset. It includes data exploration, preprocessing, feature engineering, model training, and evaluation using a Random Forest Regressor.

## 📦 Dataset

- Source: [KaggleHub - msnbehdani/mock-dataset-of-second-hand-car-sales](https://www.kaggle.com/datasets/msnbehdani/mock-dataset-of-second-hand-car-sales)
- Format: CSV
- Features include:
  - Manufacturer
  - Model
  - Fuel type
  - Engine size
  - Year of manufacture
  - Mileage
  - Price (target)

## 🧪 Project Workflow

### 1. Data Loading & Exploration
- Loaded dataset using `kagglehub`
- Visualized distributions and relationships:
  - Correlation heatmap
  - Pair plots
  - Count plots for categorical features
  - Box plots for price variation across top manufacturers

### 2. Preprocessing
- Dropped missing values
- One-hot encoded categorical features (`Manufacturer`, `Model`, `Fuel type`)
- Scaled numeric features (`Engine size`, `Year of manufacture`, `Mileage`, `Price`) using `StandardScaler`

### 3. Model Training
- Split data into training and test sets (80/20)
- Trained a `RandomForestRegressor` with 100 estimators

### 4. Evaluation Metrics
<img width="443" height="50" alt="image" src="https://github.com/user-attachments/assets/014d3ab2-7fa9-4781-ae4d-0e406283f1c3" />


> 📈 The model demonstrates excellent predictive performance with a very low MAE and near-perfect R² score.

## 📊 Visualizations

- **Correlation Heatmap**: Highlights strong relationships between numeric features.
- **Pair Plot**: Reveals linear and non-linear trends.
- **Count Plots**: Show distribution of manufacturers and fuel types.
- **Box Plot**: Compares price ranges across top manufacturers.

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- KaggleHub
