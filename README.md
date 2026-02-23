# Basic Temperature Prediction Model 

## Project Overview
This is my introductory Data Science project, completed as part of a 2-month internship. The objective was to determine if a machine learning model could accurately predict the **Temperature** of a location based solely on its **Humidity** levels. 

This project serves as the foundation for my understanding of the Linear Regression algorithm and the standard Data Science workflow.

## Dataset
The dataset consists of hourly sensor readings including pressure, humidity, and temperature.
- **Data Source:** [Download Humidity Dataset here](https://drive.google.com/file/d/1ygVqjhSpQbemqgyi4d1fpcTqz7v9lIpM/view?usp=sharing)
- **Feature Used:** `humidity` (The independent variable)
- **Target Variable:** `temperature` (The dependent variable)

## Technical Workflow
1. **Data Exploration:** Analyzed the dataset structure using Pandas and identified a negative correlation between humidity and temperature.
2. **Data Cleaning:** Identified and removed physical outliers (e.g., sensor readings of -145°C) to ensure model accuracy.
3. **Data Splitting:** Divided the data into an 80% Training set and a 20% Testing set to validate the model's performance.
4. **Model Training:** Implemented a **Simple Linear Regression** model using the `Scikit-Learn` library.
5. **Evaluation:** Evaluated the model using standard regression metrics.

## Results
The model successfully identified a trend between humidity and temperature:
- **Mean Squared Error (MSE):** 144.08
- **R-squared ($R^2$) Score:** 0.26

An $R^2$ of 0.26 indicates that while humidity is a significant predictor of temperature, other environmental factors (explored in my advanced projects) also play a role.

## How to Run
1. Clone this repository to your local machine.
2. Ensure you have a virtual environment set up.
3. Install the required libraries:
   ```bash
   pip install -r requirements.txt
