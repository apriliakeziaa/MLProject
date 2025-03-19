# MLProject
## Project Overview
This project aims to **estimate construction costs based on input parameters** such as wall area, number of floors, window quantities, door types, and other building specifications. The model is trained on historical construction data using multiple linear regression and other machine learning algorithms, which analyze the relationship between building features and final costs. The model's accuracy is evaluated using performance metrics like Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE).

## Dataset
The model uses historical construction data from Husgruppen's previous projects. Key features include:
- Wall area measurements
- Inner wall specifications
- Roof area
- Floor area
- Window quantities (standard and oversized)
- Door quantities (standard and sliding)
- Snow zone classification
- Delivery and mounting information

Note: The actual dataset cannot be shared publicly as it contains confidential business information.

## Feature Exploration
We began by analyzing the construction dataset in our [Feature_Exploration.ipnyb](https://github.com/apriliakeziaa/MLProject/blob/main/Feature_Exploration.ipynb) notebook, examining the distribution of various building specifications and their relationships with final construction costs.

## Data Preprocessing
Data Preprocessing included:
- Feature normalization using MinMaxScaler
- Data augmentation [Data_Augmentation.ipnyb](https://github.com/apriliakeziaa/MLProject/blob/main/Data_Augmentation.ipynb). We apply noise addition data augmentation to create synthetic data points

## Model Evaluation
We experimented with multiple algorithms including Linear Regression, Multilayer Perceptron neural networks, and XGBoost gradient boosting to identify the optimal cost prediction model. After comparative analysis, **the linear regression model was selected for its combination of strong performance and high interpretability**—a crucial factor for Husgruppen's stakeholders. The model was trained on augmented data with careful normalization and validation to ensure reliable cost predictions across different building specifications.

## Results and Evaluation
Linear Regression emerged as the best-performing model, providing a balance of accuracy and interpretability for construction cost estimation. **We evaluated the model using R-squared and Mean Absolute Error (MAE) metrics, achieving 81.82% of predictions within the calculated confidence interval.** For an interactive demonstration of the model's performance across different building specifications, you can download and open [Demo.html](https://github.com/apriliakeziaa/MLProject/blob/main/Demo.html) to see the estimator in action.

## Contributors:
-Eduardo Pereira

-Kezia Aprilia Sanjaya

-Juan Carlos Gonzalez

-M. Malik

-Julian Emery
