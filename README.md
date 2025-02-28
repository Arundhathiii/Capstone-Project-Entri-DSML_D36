# Electric Vehicle Price prediction Model
Dataset name: Electric Vehicle Population Data
Source: https://catalog.data.gov/dataset/electric-vehicle-population-data
Description: The Electric Vehicle Population Data dataset contains information about electric vehicles in the United States. The dataset comprises 223995 observations and 17 variables, including:
Vehicle characteristics: make, model, electric vehicle type, and base MSRP
Geographic information: county, city, state, postal code, and legislative district
Demographic data: 2020 census tract information
Utility and location data: electric utility and vehicle location
The dataset aims to provide insights into the population and characteristics of electric vehicles in the United States, which can be useful for researchers, policymakers, and industry stakeholders.

## Data Preprocessing Steps
1. Handling missing values: Replaced missing values in numerical columns with mean and categorical columns with mode.
2. Outlier detection and removal: Identified and removed outliers using the IQR method.
3. Skewness detection and removel: Identified and handled skewness using different methods
4. Encoding categorical variables: Used LabelEncoder to convert categorical variables into numerical variables.
5. Feature scaling: Scaled numerical variables using StandardScaler.
6. Feature Selection: Selecetd relevant column to predict teh Model

## Build the Model
The following machine learning models were used to predict electric vehicle prices:
1. Linear Regression: LinearRegression()
2. Decision Tree Regressor: DecisionTreeRegressor()
3. Random Forest Regressor: RandomForestRegressor()
4. Gradient Boosting Regressor: GradientBoostingRegressor()
5. Support Vector Regressor: SVR()
6. MLP Regressor: MLPRegressor()

## Model Evaluation
The accuracy of each model was evaluated, and the results showed that:
* Random Forest Regressor achieved the highest accuracy, making it the best model for predicting electric vehicle prices.

## Hyperparameter Tuning
To further improve the performance of the Random Forest Regressor model, hyperparameter tuning was performed using [GridSearchCV]. The optimal hyperparameters were selected based on the best cross-validation score.

## Pipeline Creation
A pipeline was created to streamline the modeling process. The pipeline consisted of the following steps:
1. Data preprocessing
2. Feature scaling
3. Random Forest Regressor model

## Model Saving
The trained Random Forest Regressor model was saved using [Pickle/Joblib] for future use.

## Conclusion
This project demonstrated the use of machine learning models to predict electric vehicle prices. The results showed that the Random Forest Regressor model achieved the highest accuracy, and hyperparameter tuning further improved its performance. The pipeline created can be used for future predictions.
