# Hotel Booking Price Prediction

This project predicts the **Average Daily Rate (ADR)** of hotel bookings using machine learning regression models. The objective is to estimate room prices from historical booking information and identify the factors that have the greatest impact on hotel pricing.

The project follows a complete machine learning workflow, starting from data cleaning and exploratory data analysis to feature engineering, model training, hyperparameter tuning, and model evaluation.

---

## Project Objective

Hotel room prices are influenced by several factors such as booking lead time, hotel type, customer details, room category, and booking history.

The goal of this project is to build a regression model that can accurately predict the **Average Daily Rate (ADR)** and compare multiple regression algorithms to select the best-performing model.

---

## Dataset

**Dataset:** Hotel Booking Demand Dataset

- 119,390 booking records
- 32 features
- Target Variable: **ADR (Average Daily Rate)**

The dataset contains booking information for both Resort Hotels and City Hotels.

Some of the important features include:

- Hotel Type
- Lead Time
- Market Segment
- Distribution Channel
- Customer Type
- Reserved Room Type
- Assigned Room Type
- Previous Cancellations
- Number of Adults, Children and Babies
- Deposit Type
- Special Requests

---

## Exploratory Data Analysis

Several visualizations were created to understand the data before building the models.

- Correlation Heatmap
- Pair Plot
- ADR Distribution
- Feature Correlation Analysis
- Bubble Charts
- Boxplots
- Violin Plots
- Outlier Detection

The analysis showed that variables such as lead time, room type, hotel type, number of guests, and market segment have a noticeable relationship with ADR.

---

## Data Preprocessing

The following preprocessing steps were performed before model training:

- Missing value treatment
- Duplicate removal
- Feature engineering
- Label Encoding
- Feature Scaling
- Train-Test Split

Additional features such as **Total Guests** and **Total Stay** were created to improve predictive performance.

---

## Models Implemented

### Model 1
- Linear Regression
- Cross Validation

### Model 2
- Ridge Regression
- GridSearchCV

### Model 3
- Lasso Regression
- RandomizedSearchCV

---

## Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

The evaluation metrics were used to compare model performance and determine the most suitable regression model.

---

## Results

Among the implemented models, **Ridge Regression** produced the most consistent performance after hyperparameter tuning.

Regularization improved model stability while reducing the risk of overfitting, making Ridge Regression the final model selected for ADR prediction.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

---

## Repository Structure

```
Hotel-Booking-Price-Prediction
│
├── Hotel_Booking_Price_Prediction.ipynb
├── hotel_bookings.csv
├── README.md
└── images/
```

---

## Key Takeaways

- Performed end-to-end regression analysis on a real-world hotel booking dataset.
- Compared multiple regression algorithms using the same preprocessing pipeline.
- Applied Cross Validation, GridSearchCV, and RandomizedSearchCV for model optimization.
- Built informative visualizations to understand booking behaviour and pricing patterns.
- Identified important features affecting hotel room prices.

---

## Future Improvements

Possible extensions for this project include:

- Implementing XGBoost or CatBoost Regressors
- Deploying the model using Streamlit
- Integrating SHAP for model interpretability
- Using external factors such as holidays or weather to improve predictions

---

## Author

**Dushyant Sharma**

Computer Science Undergraduate | Machine Learning Enthusiast

Feel free to connect or raise an issue if you have suggestions or feedback.
