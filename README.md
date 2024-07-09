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
This project could pinpoint areas most at risk from future temperature changes, which can help direct resources towards areas most in need of preparing for extreme temperatures.

## Tools & Libraries Used
- Python 
- Pandas
- Numpy
- Matplotlib
- Sklearn
- Seaborn
- Statsmodels


## About the Data
This project uses a dataset provided by Berkeley Earth Surface Temperature (BEST). BEST tracks temperature changes over time, and their data is constantly updated to reflect the latest trends. The focus of this project is specifically on the sub-dataset called GlobalLandTemperaturesByState.

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
7. Comparison with logistic regression for relationship analysis.

## Results

- The average temperature in the data is 8.49°C.
- The ARIMA (3,1,3) model predicts a warming trend, with the last year's average around 10.62°C, 2.13°C warmer than the current data, and an average temperature of 9.17°C. This consistency across models suggests a continuation of warming trends observed in the dataset.
- The ARIMA (3,1,3) low MSE and AIC suggest it accurately captures trends, making its predictions reliable for climate research and policy decisions. 

## Recommendations


The ARIMA (3,1,3) did a great job at forecasting temperature data. To improve our understanding, here are some next steps:

- Explore more sophisticated models and adjust the ARIMA's parameters to see if even better forecasts are possible.
- Adding more features, like CO2 emissions, could give the models a richer picture and potentially lead to more accurate predictions.
- By including other forecasting techniques, comparisons between strengths and weaknesses are possible, ultimately choosing the best approach for this project.
- While the ARIMA (3,1,3) performed well, keeping an eye on the model's performance is crucial. As new data comes in and temperature patterns change, model refinement or even changing model might be necessary to ensure forecast precision.


## Credits/Resources

https://www.kaggle.com/
https://machinelearningmastery.com/arima-for-time-series-forecasting-with-python/
https://scikit-learn.org/stable/modules/preprocessing.html
https://realpython.com/pandas-plot-python/
