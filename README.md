# Airbnb Price Prediction 
This project explores a public Airbnb dataset containing listings from New York City till March 6th 2023. I visualize the listings based on locations and other factors, and then I attempt to predict the price of Airbnb listings in NYC using some Machine Learning Models. I found that the location of the listing, and having a private room were the most important factors influencing a listing price. 

Data available at: http://insideairbnb.com/get-the-data 

## Data Cleaning 
Several steps were taken to clean to the data, impute null values and deal with outliers. Since linear regression tasks are often sensitive to outliers in the target variable, they were removed using the IQR method. Neighborhood, a categorical variable, was converted into a numerical one using the target encoder method.

## Data Visualization 
![locations](https://github.com/varshikap02/airbnb-price-pred/assets/135074696/76870a73-bc38-4d48-9681-7c9fa05035c7)

When you visualize the listings by their latitude and longitude, it resembles the map of New York City! 

## Training 
I trained 3 machine learning regression models on the dataset - Multiple Linear Regression, XG Boost Regressor, and Support Vector Regressor.  

## Results 
To measure model performance, I looked at 3 metrics - Mean Squared Error (MSE), Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE). XG Boost had the best performance across all metrics, closely followed by the Support Vector Regressor. The feature importance revealed that the location of the listing, and having a private room were the most important factors. 

<img width="423" alt="eval_metrics" src="https://github.com/varshikap02/airbnb-price-pred/assets/135074696/a55970a6-9a68-40fb-9f08-6eb2312420ba">
