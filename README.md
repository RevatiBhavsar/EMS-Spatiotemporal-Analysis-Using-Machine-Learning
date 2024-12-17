# EMS-Spatiotemporal-Analysis-Using-Machine-Learning

Overview
This project analyzes Emergency Medical Services (EMS) response times in New York City using machine learning and time series models. The primary goal is to identify spatial and temporal patterns that influence response delays and optimize resource allocation.

The project integrates:
1. Machine learning models: Random Forest, XGBoost, and Decision Trees.
2. Time series forecasting: ARIMA.
3. Exploratory Data Analysis (EDA) to uncover key trends and correlations.
4. Project Structure

The repository includes the following files:
- Notebooks-
  1. EDA.ipynb: Exploratory Data Analysis, cleaning, and preprocessing of datasets.
  2. DecisionTrees.ipynb: Implementation and evaluation of Decision Trees.
  3. RandomForestNew.ipynb: Random Forest model with hyperparameter tuning.
  4. XGBoostNew.ipynb: XGBoost model with Grid Search optimization.
  5. ARIMA.ipynb: ARIMA model for time series forecasting.

- Datasets
  1. dispatch_data_updated.csv: EMS incident dispatch data.
  2. ems_dispatch_data_exported.csv: Cleaned and processed dispatch data.
  3. Automated_Traffic_Volume_Integrated.csv: NYC traffic data for volume analysis.

-Report
RevatiB_KeerthivasanR_UC_FinalReport.pdf: Detailed report explaining methodology, results, and analysis.

- Dependencies
requirements.txt: Contains the list of Python libraries required.



Installation
Clone the repository:

bash
Copy code
git clone <repository-link>
cd EMS-Response-Analysis
Install dependencies:

|bash|
Copy code
pip install -r requirements.txt
Ensure Jupyter Notebook is installed:

|bash|
Copy code
pip install jupyterlab
Data Sources
EMS Incident Dispatch Data: NYC Open Data Portal
Traffic Density Data: Automated Traffic Volume Counts

Methodology-
1. Exploratory Data Analysis (EDA)
  -  Identified spatial hotspots and temporal delays.
  -  Analyzed incident distribution by ZIP code, time of day, and boroughs.
  -  Visualizations include correlation matrices, incident maps, and response time graphs.
2. Models Implemented
  -  Random Forest: Best-performing model with RMSE = 201.44 and R² = 0.83.
  -  XGBoost: Gradient boosting model with competitive performance.
  -  Decision Trees: Baseline model for interpretability.
  -  ARIMA: Time series forecasting for temporal patterns.
3. Model Optimization
  -  Grid Search for hyperparameter tuning.
  -  5-Fold Cross-Validation to ensure robustness.

Results
  -  Random Forest outperformed all models with an RMSE of 201.44.
  -  Temporal delays peak around 4 PM due to rush-hour traffic.
  -  Hotspot regions identified in Manhattan and the Bronx.
  -  Distance to incident and time-based features were the most significant predictors.


Instructions to Run the Code
Open a Jupyter Notebook environment:

|bash|
Copy code
jupyter lab


Load the notebooks in the following order:
  1. EDA.ipynb: Data cleaning and feature engineering.
  2. RandomForestNew.ipynb: Train and evaluate Random Forest.
  3. XGBoostNew.ipynb: Train and evaluate XGBoost.
  4. DecisionTrees.ipynb: Baseline Decision Tree model.
  5. ARIMA.ipynb: Time series forecasting.
Ensure datasets are placed in the same directory as the notebooks.

Key Visualizations
  1. Incident Distribution by Boroughs: Shows high response delays in Manhattan and the Bronx.
  2. Hourly Trends: Response delays peak at 4 PM (evening rush hour).
  3. Feature Importance: Distance to incidents and time-of-day were dominant predictors.

Future Work
  -  Integration of real-time traffic and weather data.
  -  Use of LSTM for improved temporal forecasting.
  -  Expanding analysis to other cities for generalizability.

Contributors
  1. Revati Bhavsar: EDA, baseline models, and report preparation.
  2. Keerthivasan Rajavadivel: Machine learning models, hyperparameter tuning, and result analysis.


References
Refer to the detailed report for all citations and references used in this project.

License
This project is released under the MIT License.

For further queries or contributions, feel free to reach out to the authors.
