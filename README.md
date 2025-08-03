# AICTE Internship Cycle 2 - **EV (Electric Vehicle) Charging Demand Prediction** July 2025

### Project Description

This internship project focuses on three distinct but interrelated machine learning applications:
 **EV (Electric Vehicle) Charging Demand Prediction**: This component focuses on forecasting electric vehicle charging demand based on historical data and external factors and location. 
 I have analyzed the files you provided, which seem to be related to an EV adoption forecasting project. Here's a summary of what I've found:

* `EV_Adoption_Forecasting.ipynb`: This Jupyter notebook outlines the problem of forecasting EV adoption to help urban planners. It mentions the use of a dataset from the Washington State Department of Licensing and the goal is to build a regression model. The notebook includes code for testing the saved model on a sample, and a snippet shows that the model correctly predicts the EV count for a single test sample (`Actual EVs: 1.00, Predicted EVs: 1.00`).
* `app.py`: This is a Streamlit application designed to interact with the trained model. It loads a model named `forecasting_ev_model.pkl`, sets up a web page with styling, and creates a user interface for forecasting EV adoption trends for different counties. It generates a plot showing historical and forecasted cumulative EV counts and displays the percentage growth for selected counties.
* `forecasting_ev_model.pkl`: This is a pickled Python object, likely the trained machine learning model itself. The snippet indicates it's a `RandomForestRegressor` from the `scikit-learn` library, version 1.6.1.
* `requirements.txt`: This file lists the Python libraries and their versions required to run the project. Key libraries include `numpy`, `pandas`, `scikit-learn`, `streamlit`, and `statsmodels`.
* `preprocessed_ev_data.csv`: This is a CSV file containing preprocessed data. It includes features like `Date`, `County`, `State`, `EV Total`, and engineered features such as `months_since_start`, `ev_total_lag1`, `ev_growth_slope`, etc., which are likely used as inputs for the forecasting model.
* `Electric_Vehicle_Population_By_County.csv`: This is the raw dataset used for the project. It contains information on EV populations by county, state, vehicle primary use, and date. This data was likely processed to create `preprocessed_ev_data.csv`.
* `ev-car-factory.jpg`: An image file used in the `app.py` Streamlit application.

Based on these files, the project's workflow is clear:
1.  **Data Ingestion and Preprocessing:** The `Electric_Vehicle_Population_By_County.csv` file is used as the raw data source.
2.  **Feature Engineering:** The `EV_Adoption_Forecasting.ipynb` notebook processes this data, creating new features and saving the result as `preprocessed_ev_data.csv`.
3.  **Model Training:** A `RandomForestRegressor` model is trained on the preprocessed data.
4.  **Model Persistence:** The trained model is saved as `forecasting_ev_model.pkl`.
5.  **Deployment:** A Streamlit application (`app.py`) is created to load the saved model and provide a user-friendly interface for visualizing EV adoption forecasts.

In short, the provided files constitute a complete project for forecasting EV adoption, from data preparation and model training to deployment as an interactive web application.

Together, these projects explore the use of machine learning to address key challenges in environmental monitoring, resource management, and sustainable mobility.

<img width="1157" height="833" alt="Screenshot 2025-08-04 002011" src="https://github.com/user-attachments/assets/ee50526b-5d8b-48af-9924-dac4c11e1f4a" />
<img width="1147" height="851" alt="Screenshot 2025-08-04 002109" src="https://github.com/user-attachments/assets/0e9549b4-fdee-4aac-bd17-de8f06c4b80b" />
<img width="1150" height="852" alt="Screenshot 2025-08-04 002218" src="https://github.com/user-attachments/assets/7f989d8a-3264-4a93-8819-a506ad6bd5e5" />


## Badges

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

