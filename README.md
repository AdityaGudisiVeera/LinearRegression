# 🏠 House Price Prediction

## 📌 Overview
This project builds a basic machine learning model to predict house prices using a dataset. It includes data preprocessing, feature encoding, and training a linear regression model.

---

## 📂 Dataset
- Dataset used: `HousePricePrediction.csv`
- Loaded using pandas

---

## ⚙️ Steps Performed

### 1. Import Libraries
- pandas
- numpy
- sklearn
- seaborn
- matplotlib

---

### 2. Load Data
- Dataset is loaded using:
  ```python
  pd.read_csv("HousePricePrediction.csv")
  ```

---

### 3. Data Exploration
- Displayed first few rows using:
  ```python
  house_data.head()
  ```
- Calculated correlation matrix
- Identified features correlated with `SalePrice`

---

### 4. Data Cleaning
- Filled missing values in `SalePrice` with mean
- Filled remaining missing values with 0

---

### 5. Feature Engineering
- Converted categorical variables into numerical using:
  ```python
  pd.get_dummies()
  ```

---

### 6. Feature Selection
- Dropped unnecessary columns:
  - Id
  - BsmtFinSF2
  - SalePrice (target)
  - MSSubClass
- Defined:
  - X → input features
  - Y → target (SalePrice)

---

### 7. Model Training
- Used Linear Regression model
- Split data into training and testing sets (80/20)
- Trained model using:
  ```python
  LinearRegression()
  ```

---

### 8. Model Evaluation
- Evaluated using R² score:
  ```python
  r2_score(Y_test, predictions)
  ```

---

### 9. Visualization
- Plotted Actual vs Predicted values using seaborn
- Used regression plot to visualize model performance

---

## 🛠️ Libraries Used
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib
