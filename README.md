# Co2-emission-Prediction-for-Vehicles

A machine learning project to predict vehicle CO₂ emissions (g/km) using vehicle specifications and fuel consumption data. The project compares Linear Regression, Random Forest, and XGBoost regression models.

Project Overview

This project uses machine learning techniques to estimate vehicle CO₂ emissions based on vehicle characteristics. It includes data preprocessing, exploratory data analysis (EDA), model training, and performance evaluation.

The trained XGBoost model is saved for reuse and integrated into a Streamlit web application for interactive predictions.

Dataset

- Dataset: CO₂ Emissions in Canada
- File: "CO2 Emissions_Canada.csv"
- Task: Regression
- Target variable: CO₂ emissions (g/km)

The dataset contains vehicle specifications and fuel consumption information used to train and evaluate the models.

Machine Learning Models

The following regression algorithms were implemented:

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

Model Performance

The models were trained using 5,908 samples and evaluated on 1,477 test samples.

Model| R² Score| MAE (g/km)| RMSE (g/km)
Linear Regression| 0.8773| 13.5173| 20.5407
Random Forest| 0.9680| 4.0901| 10.1810
XGBoost| 0.9711| 4.3929| 9.9685

Results and Observations

- Linear Regression: Achieved an R² score of 0.8773, with an MAE of 13.5173 g/km and an RMSE of 20.5407 g/km.
- Random Forest: Achieved an R² score of 0.9680, with an MAE of 4.0901 g/km and an RMSE of 10.1810 g/km.
- XGBoost: Achieved an R² score of 0.9711, with an MAE of 4.3929 g/km and an RMSE of 9.9685 g/km.

XGBoost achieved the highest R² score and lowest RMSE, while Random Forest achieved the lowest MAE among the three models.

Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Joblib
- Streamlit

Project Structure

CO2-emission-Prediction-for-Vehicles/
│
├── CO2 Emissions_Canada.csv
├── co2_emission_per_km_git.ipynb
├── xgb_model.pkl
├── app.py
├── requirements.txt
└── README.md

Installation and Usage

1. Clone the repository

git clone https://github.com/rajravishantanu-svg/CO2-emission-Prediction-for-Vehicles.git

2. Navigate to the project directory

cd CO2-emission-Prediction-for-Vehicles

3. Install dependencies

pip install -r requirements.txt

4. Run the Jupyter Notebook

jupyter notebook

Open the notebook to explore the data preprocessing, EDA, model training, and evaluation workflow.

Streamlit Web Application

The project includes a Streamlit web application for interactive vehicle CO₂ emission prediction using the trained XGBoost model.

The application allows users to:

- Enter vehicle specifications and fuel consumption data.
- Predict CO₂ emissions using the trained XGBoost model.
- View predicted emissions in g/km.

Run Locally

streamlit run app.py

Online Deployment

The Streamlit application can be deployed using "Streamlit Community Cloud" (https://share.streamlit.io/).

To deploy:

1. Push the project files to GitHub.
2. Sign in to Streamlit Community Cloud.
3. Connect your GitHub repository.
4. Select "app.py" as the application entry point.
5. Deploy the application.

Future Improvements

- Add interactive visualizations for vehicle emission trends.
- Compare predictions from multiple machine learning models.
- Improve the user interface and provide downloadable prediction results.
- Explore model interpretability using feature importance.

Author

Ravi Raj Shantanu
B.E. Chemical Engineering
Dr. S. S. Bhatnagar University Institute of Chemical Engineering & Technology, Panjab University, Chandigarh

"GitHub Profile" (https://github.com/rajravishantanu-svg)
