Personal Fitness Tracker

Overview

The Personal Fitness Tracker is a Streamlit-based web application that predicts the number of calories burned during exercise based on user input parameters like age, BMI, exercise duration, heart rate, body temperature, and gender. The app also compares the user's metrics against a dataset to provide additional insights.

Features

Accepts user inputs through a sidebar for Age, BMI, Duration, Heart Rate, Body Temperature, and Gender.

Uses Random Forest Regressor to predict the number of calories burned.

Displays a comparison of the user's metrics with others from the dataset.

Shows similar results from the dataset based on predicted calories burned.

Technologies Used

Python

Streamlit

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

Dataset Information

The application uses two CSV files:

calories.csv: Contains information on the calories burned by users.

exercise.csv: Contains details like User ID, Gender, Age, Height, Weight, Duration, Heart Rate, and Body Temperature.

These datasets are merged on User_ID to create a comprehensive dataset for model training.

Model Training

The Random Forest Regressor is trained on 80% of the dataset, while 20% is used for testing.

Key features used: Gender, Age, BMI, Duration, Heart Rate, and Body Temperature.

BMI is calculated as Weight / (Height/100)^2.

Installation

Clone the repository:

git clone <repository-url>

Install the required dependencies:

pip install streamlit numpy pandas matplotlib seaborn scikit-learn

Ensure the CSV files (calories.csv and exercise.csv) are in the same directory as app.py.

Run the Streamlit application:

streamlit run app.py

Usage

Adjust the input parameters in the sidebar.

View the predicted calories burned and a comparison of your metrics.

Explore similar data from the dataset for a broader perspective.

Future Enhancements

Add authentication for personalized user tracking.

Implement advanced analytics like time-series tracking of fitness data.

Integrate more advanced machine learning models for enhanced prediction accuracy.

Contributing

Contributions are welcome! Please open an issue or submit a pull request for suggestions.

License

This project is licensed under the MIT License.
