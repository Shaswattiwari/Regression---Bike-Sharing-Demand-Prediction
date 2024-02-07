# Seoul Bike Rental Analysis and Prediction

Seoul Bike Rental Analysis and Prediction is a Python project that combines the predictive modeling approach with data analysis of historical bike rental data from Seoul. The project aims to forecast bike rental counts while also providing insights into the underlying data patterns and distributions. Below is a unified overview of the project, integrating elements from both readme files:

## Abstract

The Seoul Bike Rental Analysis and Prediction project focus on forecasting the number of rented bikes in Seoul using various features such as temperature, humidity, wind speed, and more. It leverages deep learning models like GRU, CNN, and LSTM for prediction, while also incorporating anomaly detection techniques to improve model accuracy. Additionally, the project includes comprehensive data analysis and visualization to understand the historical bike rental patterns.

## Introduction

The project begins with the installation of required Python packages and libraries using pip. It sets up the environment for data processing, modeling, and visualization. Additionally, warning filters are applied to suppress unnecessary warnings during execution.

## Data Preparation for Modeling

The dataset, loaded from "SeoulBikeData.CSV.csv," is preprocessed to aggregate hourly data into daily summaries. Categorical features like Seasons and Holiday are converted into a suitable format. Missing values are handled, and exploratory data analysis (EDA) is performed using Altair to visualize the distribution of key variables.

## Modeling Approach

The predictive modeling approach involves training three deep learning models: GRU, CNN, and LSTM. Before training, categorical columns are one-hot encoded, and an autoencoder is utilized for anomaly detection. Outliers are removed to improve model robustness.

## Prediction Results

The code trains GRU, CNN, and LSTM models on the preprocessed data and makes predictions for a future time period. The predictions are then aggregated and presented in a visual format using Altair. The results showcase the predicted values alongside the actual bike rental counts, providing insights into the model's performance.

## Dependencies

To run this project, ensure you have the following dependencies installed:

- Pandas
- TensorFlow
- scikit-learn
- Keras
- Matplotlib
- Funcyimpute
- shap
- PyOD
- eli5
- statsmodels
- altair_viewer
You can install these dependencies using pip:

```bash
pip install pandas tensorflow scikit-learn keras matplotlib Funcyimpute shap PyOD eli5 statsmodels altair_viewer
```
## How to Run
Make sure you have the necessary CSV file (SeoulBikeData.CSV.csv) with the bike rental data located in the same folder as the Python script. Then proceed to run the code.

## Conclusion

The Seoul Bike Rental Analysis and Prediction project demonstrates the application of deep learning techniques for time series forecasting and anomaly detection. By combining predictive modeling with comprehensive data analysis, the project offers insights into historical bike rental patterns and forecasts future rental demand accurately.
