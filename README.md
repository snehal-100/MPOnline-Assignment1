# Medical Insurance Cost Prediction using Multiple Linear Regression

**Author:** Akshat Garg  

**Registration Number:** 23BCE10641  

**Application Number:** IN26011052

**Batch Number:** 1A

**Email ID:** akshat.23bce10641@vitbhopal.ac.in

## Objective
The objective of this project is to develop a Multiple Linear Regression model to estimate medical insurance charges based on individual health and personal features.

## Dataset Link
- [Kaggle: Medical Cost Personal Insurance Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)

## Libraries Used
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `kaggle`

## Methodology
1. **Data Understanding**: Loaded the dataset, identified numerical/categorical variables, and inspected target values.
2. **Data Preprocessing**: Verified missing values and encoded categorical features (`sex`, `smoker`, `region`) using one-hot encoding (`drop_first=True`).
3. **Data Splitting**: Split the data into 80% training set and 20% testing set using `train_test_split`.
4. **Model Development**: Fitted a `LinearRegression` model from `scikit-learn` using all features.
5. **Model Evaluation**: Evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score, alongside an actual vs. predicted scatter plot.

## Results
- **R² Score:** ~0.78
- **Primary Cost Drivers:** Smoking status, age, and BMI.

## Conclusion
Multiple Linear Regression effectively captures general trends in insurance charges ($R^2 \approx 0.78$). However, its main limitation is the inability to model complex non-linear feature interactions (e.g., compound risk of high BMI combined with smoking). Future work could leverage non-linear ensemble models like Random Forest or XGBoost.
