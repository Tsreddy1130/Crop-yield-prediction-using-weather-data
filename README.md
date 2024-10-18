# Weather-Driven Crop Yield Prediction Using Machine Learning
This project focuses on the development of a machine learning-based crop yield prediction system using historical data from Maharashtra's rice crop production between 1997 and 2019. The system incorporates environmental factors such as rainfall, maximum temperature, and district-level area characteristics to predict rice production. By leveraging multiple regression models, including Decision Tree, K-Nearest Neighbor (KNN), and Random Forest, the project aims to identify the most accurate method for forecasting yield based on weather inputs and geographical distinctions.
 ## Dataset Overview
•	Source: The dataset contains crop data for rice in Maharashtra, including attributes like district name, crop year, production, rainfall, maximum temperature, etc.
•	Rows: 926
•	Columns: 10 (initially), later reduced by dropping irrelevant columns like 'State_Name' and 'Crop.'
## Data Preprocessing
•	Dropped columns: 'State_Name' and 'Crop' as they are not necessary for the prediction task.
•	Handling categorical data:
o	Categorical columns such as 'District_Name' and 'Season' were encoded using LabelEncoder and OneHotEncoder to convert them into numerical format suitable for machine learning models.
•	Data splitting: The data was split into features (X) and target variable (y) representing production, followed by a train-test split with 90% data for training and 10% for testing.
## Model Building
### Decision Tree Regressor:
o	The Decision Tree model was trained on the training data.
o	Performance Metrics:
	Mean Absolute Error (MAE): Measures average error.
	Mean Squared Error (MSE): Measures error squared.
	Root Mean Squared Error (RMSE): Square root of MSE.
	R² Score: Measures the model's accuracy.
	Visual comparison between real and predicted values was plotted.
### K-Nearest Neighbor (KNN) Regressor:
o	KNN model was implemented with n_neighbors=3.
o	Similar error metrics (MAE, MSE, RMSE) and R² score were computed and visualized.
### Random Forest Regressor:
o	Random Forest model was trained using 1000 estimators.
o	Same error metrics were calculated, and predictions were visualized.
## Model Evaluation
•	All three models (Decision Tree, KNN, Random Forest) were evaluated based on their performance metrics, particularly the R² score, which was used to represent the accuracy of each model:
o	KNN: Highest accuracy.
o	Decision Tree: Moderate performance.
o	Random Forest: Lower accuracy compared to the other two models.
•	Visualization: Bar plots were created to compare the accuracy (R² score as a percentage) across the models.
## Conclusion
•	K-Nearest Neighbor  outperformed both the Decision Tree and Random Forest Regressor Regressors in terms of accuracy, making it the best model for predicting crop yield based on the dataset.
•	The visual comparison provides clear insights into how the models performed relative to each other.
![image](https://github.com/user-attachments/assets/175a3de5-10a7-4aa5-a1cb-d75c8317c126)

