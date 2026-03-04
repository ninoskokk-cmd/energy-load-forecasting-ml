# energy-load-forecasting-ml
Hourly energy load prediction using Random Forest Regressor and multi-city weather data. Achieved 98% accuracy (MAE: 284 MW).
This project focuses on predicting hourly national electricity demand using historical consumption and weather data. Accurate load forecasting is crucial for grid stability, energy trading, and integrating renewable energy sources.

The model analyzes how environmental factors (temperature, humidity, wind speed) across 5 major cities influence the total electrical load.

Tech Stack
Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn

Machine Learning: Scikit-Learn (Random Forest Regressor)

Environment: Jupyter Notebook

 Methodology
Data Engineering: Merged multi-city weather datasets with grid energy data. Handled missing values and performed feature extraction from timestamps.

Time-Series Split: To ensure realistic evaluation and avoid data leakage, a chronological split was used:

Training Set: 2015 – 2017

Test Set: 2018 (Unseen future data)

Model: Implemented a Random Forest Regressor, which effectively captures non-linear relationships between weather variables and energy demand.

Key Results
Mean Absolute Error (MAE): 284.27 MW

Root Mean Squared Error (RMSE): 401.71 MW

Accuracy: The model achieved high precision, following daily and seasonal demand cycles with an error margin of approximately ~1-2% relative to the average load.
