# 🏠 Ames Housing Price Prediction

## 📚 Project Overview
This project applies supervised learning techniques to predict the sale prices of houses based on the Ames Housing dataset.  
We use regression models to estimate SalePrice from a set of features describing each house, including quality, size, and year built.

The goal is to build accurate, generalizable models to assist in real-estate price estimation tasks.

---

## 📈 Machine Learning Approach
- **Type of learning**: Supervised Learning
- **Task**: Regression
- **Models Used**:
  - Linear Regression
  - Ridge Regression (with hyperparameter tuning)
  - Lasso Regression (with hyperparameter tuning)

Regularization techniques (Ridge and Lasso) were employed to reduce overfitting and enhance model performance.  
Hyperparameters were optimized using GridSearchCV.

---

## 📊 Results Summary
| Model             | RMSE      | MAE       | R² Score |
|:------------------|:---------|:---------|:--------|
| Linear Regression | 0.1299   | 0.0792    | 0.9089  |
| Random Forest     | 0.1240   | 0.0856    | 0.9169  |
| AdaBoost          | 0.1693   | 0.1333    | 0.8452  |
| Decision Tree     | 0.1660   | 0.1192    | 0.8510  |
| KNN               | 0.2005   | 0.1408    | 0.7827  |
| Ridge             | 0.1126   | 0.0782    | 0.9315  |
| Lasso             | 0.1135   | 0.0776    | 0.9303  |

🏆 **Best Model**: Ridge Regression  
- Ridge achieved the lowest RMSE and highest R², indicating the best predictive performance.

---

## 🛠️ Project Structure

| File/Folder | Description |
|:------------|:------------|
| `AmesHousing_ML_Notebook.ipynb` | Full data cleaning, EDA, modeling, and evaluation |
| `README.md` | Project overview and documentation |
| `requirements.txt` | Project dependencies |
---

## 🗂️ Dataset Information
- **Source**: [Ames Housing dataset](https://www.kaggle.com/datasets/prevek18/ames-housing-dataset)
- **Size**: 2930 rows × 82 features
- **Description**: Features describe residential houses in Ames, Iowa (e.g., OverallQual, GrLivArea, GarageCars, TotalBsmtSF).

---

## 🚀 How to Run
1. Clone this repository:
    ```bash
    git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
    ```
2. Install required libraries:
    ```bash
    pip install -r requirements.txt
    ```
3. Open the Jupyter Notebook:
    ```bash
    jupyter notebook AmesHousing_ML_Notebook.ipynb
    ```
4. Run all cells to reproduce the full analysis.

---

## 🎯 Future Work
- Try ensemble methods (Gradient Boosting, XGBoost) for potentially better performance.
- Explore feature scaling and polynomial features for more complex relationships.
