# Chennai ERA5 Weather Forecasting

Hourly temperature forecasting for Chennai using ERA5
reanalysis data, time-series analysis, and machine learning.

## Project Overview

This project analyses hourly weather data from 2020–2025
and compares forecasting models using a chronological
training and testing strategy.

## Dataset

- Source: Copernicus Climate Data Store (ERA5)
- Location: Chennai, India
- Period: 2020–2025
- Temporal resolution: Hourly
- Target variable: 2-metre air temperature

## Methods

- Data cleaning and quality checks
- Exploratory Data Analysis (EDA)
- Time-based train-test split
- Persistence baseline
- Linear Regression
- Autoregressive model AR(3)
- Long Short-Term Memory (LSTM)

## Model Evaluation

Models are evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

| Model | MAE (°C) | RMSE (°C) |
|---|---:|---:|
| Persistence | 0.412 | 0.598 |
| Linear Regression | 0.412 | 0.591 |
| AR(3) | 0.367 | 0.532 |
| LSTM | 0.350 | 0.453 |

LSTM achieved the lowest reported errors among the
evaluated models on the 2025 test period.

## Tools and Libraries

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

## How to Run

1. Download or clone this repository.
2. Install the required Python libraries.
3. Open the notebook in Jupyter.
4. Configure the path to your ERA5 CSV dataset.
5. Run the notebook cells in order.

## Limitations

- Evaluation focuses on one-hour-ahead temperature forecasts.
- ERA5 reanalysis is not the same as direct station observations.
- Results are specific to the selected location, data period,
  features, and test setup.

## Future Improvements

- Evaluate rainfall forecasting.
- Compare predictions with weather-station observations.
- Test longer forecast horizons.
- Explore additional time-series models.

## Author

Climate Data Science Project
