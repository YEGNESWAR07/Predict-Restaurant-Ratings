# Predict-Restaurant-Ratings
markdown
# Restaurant Rating Prediction Model

## Description
This project implements a machine learning model to predict restaurant ratings using various features such as location, cuisine type, cost, and service attributes. The model uses Random Forest Regression with automated feature preprocessing and hyperparameter tuning to provide accurate rating predictions.

## Workflow
1. Data Preprocessing
   - Load restaurant data from CSV
   - Remove irrelevant identifiers (Restaurant ID, Name)
   - Handle missing values in numeric and categorical features
   - Scale numeric features and encode categorical variables

2. Model Pipeline
   - Split data into training (80%) and testing (20%) sets
   - Create preprocessing pipeline with numeric and categorical transformers
   - Train Random Forest Regressor
   - Perform hyperparameter tuning using GridSearchCV

3. Evaluation & Analysis
   - Calculate performance metrics (MSE, RMSE, R²)
   - Generate feature importance visualization
   - Identify optimal model parameters
## Libraries Used
- `pandas`: Data manipulation and analysis
- `numpy`: Numerical operations
- `scikit-learn`: Machine learning algorithms and preprocessing
  - `RandomForestRegressor`: Main prediction algorithm
  - `Pipeline`: Streamlined data processing
  - `ColumnTransformer`: Feature-specific transformations
- `matplotlib`: Visualization of feature importance

## Algorithm Choice: Random Forest Regressor
Selected for its advantages:
- Handles both numerical and categorical features effectively
- Robust to outliers and non-linear relationships
- Provides feature importance analysis
- Reduces overfitting through ensemble learning
- Performs well with default parameters
  
## Requirements
pandas>=1.0.0
numpy>=1.19.0
scikit-learn>=0.24.0
matplotlib>=3.3.0

## Installation
bash
pip install -r requirements.txt

## Usage
1. Prepare your data in CSV format with required columns:
   - City
   - Cuisines
   - Average Cost for two
   - Has Table booking
   - Has Online delivery
   - Votes
   - Aggregate rating

2. Run the model:
     python restaurant_rating_predictor.py

## Model Features
- Automated handling of missing values
- Feature scaling and encoding
- Hyperparameter optimization
- Feature importance analysis
- Model persistence for future predictions

## Performance Metrics
- MSE (Mean Squared Error)
- RMSE (Root Mean Squared Error)
- R² (R-squared) score

## Contributing
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License
MIT License
