
# Laptop Price Prediction Using Regression

## Project Overview
This project aims to predict the prices of laptops using various regression models. The dataset contains features such as brand, specifications, and other attributes to train the model to estimate the price accurately. The goal is to experiment with multiple machine learning algorithms and compare their performance to achieve the best prediction accuracy.

## Dataset
- **Dataset Name**: `final_data`
- **Number of Rows**: 7,500
- **Target Column**: `buynow_price`
- **Features**: 
  - Brand  
  - Processor  
  - RAM  
  - Storage Type (HDD/SSD)  
  - Graphics Card  
  - Screen Size, etc.

### Main Libraries:
- **pandas**: Data manipulation  
- **numpy**: Numerical operations  
- **scikit-learn**: Machine learning algorithms  
- **xgboost**: XGBoost regressor for optimized predictions  
- **matplotlib** & **seaborn**: Visualization tools  

## Model Overview
The project compares several models to predict laptop prices:
1. **XGBoost Regressor** (Best performing)  
2. **Random Forest Regressor**  
3. **Decision Tree Regressor**  
4. **Neural Network (MLP)**  
5. **K-Nearest Neighbors (KNN)**  
6. **Lasso Regression**
7. **Ridge Regression**
8. **Elastic Net Regression**
9. **Polynomial Regression**

## Results
The performance of various regression models used for laptop price prediction is summarized in the table below:

| Model                    | ME      | RMSE     | MAE     | MPE     | MAPE   |
|--------------------------|---------|----------|---------|---------|--------|
| Linear Regression        | 32.90   | 857.43   | 610.22  | -2.53   | 17.30  |
| Random Forest            | -7.11   | 598.19   | 363.46  | -2.15   | 9.79   |
| Decision Tree            | -13.92  | 650.51   | 371.36  | -2.07   | 10.24  |
| XGBoost                  | 17.67   | 566.94   | 372.11  | -1.16   | 9.96   |
| Support Vector Regression | 163.51 | 1024.94  | 451.65  | 1.65    | 11.44  |
| Neural Network           | 18.52   | 806.39   | 522.35  | -2.29   | 13.96  |
| KNN Regressor            | 24.63   | 654.54   | 427.05  | -1.48   | 11.29  |
| Lasso Regression         | 32.66   | 857.18   | 610.16  | -2.54   | 17.30  |
| Ridge Regression         | 32.92   | 857.39   | 610.23  | -2.53   | 17.30  |
| Elastic Net Regression   | 32.42   | 856.28   | 609.46  | -2.59   | 17.27  |
| Polynomial Regression    | 33.57   | 857.39   | 610.54  | -2.47   | 17.33  |

### Key Insights:
- **XGBoost Regressor** achieved the lowest RMSE (566.94) and MAPE (9.96), making it the best-performing model in this project.  
- **Random Forest** performed closely behind XGBoost with a MAPE of 9.79.  
- **Support Vector Regression** had the highest error metrics, indicating poor performance for this task.  
- **Neural Networks** and **KNN Regressor** demonstrated moderate performance but were outperformed by XGBoost and Random Forest.  
- Linear, Ridge, Lasso, and Polynomial regressions yielded higher error metrics, suggesting they might not be the best fit for predicting laptop prices.

These results suggest that **ensemble models like XGBoost and Random Forest** are more effective for predicting laptop prices compared to simpler linear and polynomial models.

- **XGBoost Regressor** achieved the lowest MAPE of **15-20%**.  
- Random Forest and Decision Tree performed decently but were slightly outperformed by XGBoost.  
- Neural Network and KNN models had lower performance due to higher variance and computational limitations.  

## Future Improvements
- **Feature Engineering**: Add new features like laptop brand reputation or regional pricing.  
- **Hyperparameter Tuning**: Use GridSearchCV or RandomizedSearchCV for better model performance.  
- **Ensemble Methods**: Combine multiple models to further enhance accuracy.  
