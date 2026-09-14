# Time-Series-Analysis-of-Climate-Change-using-ARIMA-Model

## Objective
This project aims to analyse Earth's continuously warming climate. Using time series analysis to uncover hidden patterns in temperature data. The objective is to interpret the patterns and changes in Earth's temperature, a vital process in understanding the impact of climate change and mapping out a cooler trajectory for the future.


## Motivation
The Earth's climate is changing, and the future feels uncertain. But what if we could peek ahead? Accurately predicting future temperature fluctuations is the key to preparing for the impact of climate change. This project excites me because it uses the ARIMA model, a powerful tool, to unlock the secrets driving our climate. Forecasting future temperature changes empowers us to adapt and fight back against the effects of climate change. Using data, we can move beyond inspiration and create tangible solutions.

## Project Objectives
The primary objectives of this project are to:
- Develop an ARIMA model to predict future temperatures.
- Validate the model’s accuracy and refine it for better performance.
- Compare the results with other statistical models.
  
## Actionable Insights 
This project provides insights into historical temperature trends and future projections, which can help policymakers and environmental organisations anticipate the impacts of climate change, prioritise actions to mitigate potential risks, and adapt strategies to better manage the challenges of rising temperatures.

## Tools & Libraries Used
- Python 
- Pandas
- Numpy
- Matplotlib
- Sklearn
- Seaborn
- Statsmodels


## About the Data
This project uses historical land-temperature data compiled by Berkeley Earth. The selected file, GlobalLandTemperaturesByState.csv, contains temperature observations for individual states and countries over time. The notebook prepares and aggregates these records into a chronological series for time-series analysis. It should therefore be understood as an analysis derived from state-level land-temperature observations rather than a direct measurement of the Earth’s single global average temperature.

- DT: Date of the temperature record.
- Average temperature:	Average temperature in Celsius for the state on the corresponding date.
- Average temperature uncertainty:	95% confidence interval around the average temperature (capturing measurement uncertainty).
- State:	The specific state for which temperature data is recorded.
- Country:	The specific country for which temperature data is recorded.

[Click here to access the dataset on Kaggle](https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data?select=GlobalLandTemperaturesByState.csv)

## Methodology

1. Data preprocessing.
2. Model selection and parameter tuning.
3. Model Estimation.
4. Model Validation.
5. Forecasting.
6. Interpretation and Application.
7. The linear regression benchmark, evaluated on the same held-out period as ARIMA, performs far worse (R² ≈ -12.4, test MSE 2.70) than ARIMA(3,1,3)'s test MSE of 0.427 — the training window's noisiest, sparsest decades pull the fitted line well below the accelerating warming seen later in the record, confirming ARIMA's forecasting captures meaningfully more of the real pattern than a naive linear trend.


## Results

- The average temperature in the data is 8.49°C.
- The mean temperature across the analysed dataset is 8.49°C. The ARIMA (3,1,3) model produces a forecast of approximately 9.43°C at the end of the one-year forecast horizon. This forecast is consistent with the broader warming trend identified in the historical series. However, the dataset-wide mean should not be interpreted as the temperature immediately preceding the forecast.
- Among the candidate specifications evaluated, the ARIMA (3,1,3) model produced favourable MSE and AIC results. These measures suggest that the model captured useful patterns in the analysed series. However, AIC measures relative model fit rather than guaranteeing future forecast accuracy, so the results should be interpreted alongside validation performance, residual diagnostics and forecast uncertainty. 

## Recommendations


The ARIMA (3,1,3) did a great job at forecasting temperature data. To improve our understanding, here are some next steps:

- Explore more sophisticated models and adjust the ARIMA's parameters to see if even better forecasts are possible.
- Adding more features, like CO2 emissions, could give the models a richer picture and potentially lead to more accurate predictions.
- By including other forecasting techniques, comparisons between strengths and weaknesses are possible, ultimately choosing the best approach for this project.
- While the ARIMA (3,1,3) performed well, keeping an eye on the model's performance is crucial. As new data comes in and temperature patterns change, model refinement or even changing model might be necessary to ensure forecast precision.


## Credits/Resources

- https://www.kaggle.com/
- https://machinelearningmastery.com/arima-for-time-series-forecasting-with-python/
- https://scikit-learn.org/stable/modules/preprocessing.html
- https://realpython.com/pandas-plot-python/
