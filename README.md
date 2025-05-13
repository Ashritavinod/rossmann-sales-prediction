#  Rossmann Sales Prediction using XGBoost

This project predicts daily sales for Rossmann drug stores using historical data and store information. It uses machine learning techniques including feature engineering, model tuning, and XGBoost regression.

##  Objective
To develop an accurate sales prediction model using historical sales data, store attributes, and promotion information.

---

## 🛠 Workflow

### 1. Data Loading & Merging
- Loaded `train.csv`, `test.csv`, and `store.csv`
- Merged to create a unified dataset

### 2. Exploratory Data Analysis (EDA)
- Inspected data using `.info()` and `.describe()`
- Removed rows with zero sales (when stores were closed)

### 3. Feature Engineering
- **Date Parsing**: Extracted year, month, day, and week
- **Competition Features**: Duration since competitor opened
- **Promotion Features**: Promo2 duration and current activity
- **Missing Values**: Filled `CompetitionDistance` with a high value
- **Encoding**: One-hot encoded categorical variables
- **Scaling**: Applied `MinMaxScaler` to numerical features

### 4. Model Training
- Used `XGBRegressor` for prediction
- Visualized decision trees using `plot_tree`
- Analyzed feature importance

### 5. Model Evaluation
- Evaluated with Root Mean Squared Error (RMSE)
- Applied **KFold Cross Validation**
- Tuned hyperparameters for improved performance

### 6. Final Model
- Trained final model with tuned hyperparameters
- Predicted on test dataset

---

##  Getting Started

1. Clone the repo:
```bash
git clone https://github.com/your-username/rossmann-sales-prediction.git
cd rossmann-sales-prediction


