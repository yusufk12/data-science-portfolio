# Time Series Analysis using Prophet

## Project Overview

This project involves analyzing trends in health metrics over time using the Prophet model. The objective is to forecast the daily steps recorded by a fitness tracker, identify trends and seasonal patterns, and evaluate the model's performance. The analysis includes data cleaning, preprocessing, removing outliers, and generating forecasts. Performance metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE) are calculated to evaluate the model's accuracy.

## Dataset

The dataset contains daily records of steps, distance, run distance, and calories burned. The data spans several years and provides a comprehensive view of physical activity over time.

### Columns:
- **date:** The date of the record.
- **steps:** The number of steps taken.
- **distance:** The distance covered in meters.
- **rundistance:** The distance covered while running in meters.
- **calories:** The number of calories burned.

## Methodology

### 1. Data Preprocessing
- Converted the `date` column to datetime format and set it as the index.
- Checked for and handled missing values using forward fill method.
- Set the frequency of the datetime index to daily.

### 2. Outlier Detection and Removal
- Identified outliers using the Interquartile Range (IQR) method.
- Removed outliers to ensure the model is not influenced by extreme values.

### 3. Prophet Model
- Prepared the data for the Prophet model.
- Split the data into training (80%) and testing (20%) sets.
- Initialized and fit the Prophet model on the training data.
- Created a dataframe for future dates including the test period and generated forecasts.

### 4. Performance Metrics
- Calculated performance metrics including MAE, MSE, and RMSE to evaluate the model's accuracy.

## Results

### Forecast Plot

![Prophet Forecast (No Outliers)](path/to/your/forecast_plot.png)

### Performance Metrics

- **Mean Absolute Error (MAE):** 4039.28
- **Mean Squared Error (MSE):** 32805740.11
- **Root Mean Squared Error (RMSE):** 5727.63

The performance metrics indicate an improvement in model accuracy after outlier removal. The forecast plot shows the predicted values with confidence intervals, capturing the overall trend and seasonal patterns in the data.

## Conclusion

The Prophet model effectively identified trends and seasonal patterns in the daily steps data. Removing outliers improved the model's accuracy, as indicated by the performance metrics. This project demonstrates the importance of data preprocessing and the capability of the Prophet model in time series forecasting.

## Files in This Repository

- **TimeSeriesAnalysis.ipynb:** The Jupyter Notebook containing the code for the time series analysis and forecasting using the Prophet model.
- **README.md:** This README file describing the project.

## How to Run the Notebook

1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Open the `TimeSeriesAnalysis.ipynb` notebook using Jupyter Notebook or JupyterLab.
4. Run the cells in the notebook to see the analysis and results.

## Author

**Yusuf Khan**

- [LinkedIn](https://www.linkedin.com/in/yusufkhan)
- [GitHub](https://github.com/yusufkhan)

Feel free to reach out if you have any questions or feedback!
