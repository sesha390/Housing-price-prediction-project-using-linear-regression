# Housing-price-prediction-project-using-linear-regression
This project involves predicting housing prices for Bengaluru region using Linear regression. This project involves the data cleaning and preparation, Feature Engineering, outlier detection and imputing them, train-test split, dummy variables with one-hot encoding,  training the model, evaluating the model and picking the best model.

I worked on a real-world Machine Learning project where the goal was to predict house prices in Bangalore based on features like location, total square footage, number of bedrooms, and bathrooms.

I started with data cleaning. The raw dataset had missing values, inconsistent formats for square footage, and some unrealistic entries. I cleaned the data by removing null values, converting ranges into numerical values, and filtering out properties that didn’t make logical sense.

Next, I performed feature engineering. I created important features such as price per square foot, extracted the number of bedrooms from the size column, and ensured numerical features were in a format suitable for machine learning models. This step helped improve the model’s ability to learn meaningful patterns.

Then I handled outlier detection and removal. I removed extreme price-per-square-foot values using statistical methods like mean and standard deviation, applied separately for each location. I also removed logical outliers, such as cases where a 3-bedroom apartment was priced lower per square foot than a 2-bedroom apartment in the same location, and properties where the number of bathrooms was unrealistic compared to bedrooms.

After that, I worked on dimensionality reduction and encoding. Since location is a categorical variable, I used one-hot encoding to convert locations into numerical features. To avoid the curse of dimensionality, I grouped rare locations into an “other” category, which helped reduce noise and improve model performance.

For model building, I trained multiple regression models including Linear Regression, Lasso Regression, and Decision Tree Regressor. I evaluated them using R² score and cross-validation to ensure the model generalized well to unseen data.

I used GridSearchCV to systematically tune hyperparameters and compare models instead of choosing them manually. This helped me identify Linear Regression as the best performing model for this dataset.

Finally, I built a prediction pipeline where a user can input location, square footage, number of bathrooms, and bedrooms, and the model returns a predicted house price. I also saved the trained model and feature columns for future deployment.

Overall, this project gave me hands-on experience with the complete Machine Learning pipeline, from raw data to a trained and evaluated model, following real industry practices.
