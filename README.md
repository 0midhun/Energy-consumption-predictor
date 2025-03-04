# World Energy Consumption Prediction Project

## Overview
This machine learning project predicts primary energy consumption for different countries using various features like population, GDP, and energy source consumption. The project demonstrates a simple yet effective approach to understanding energy consumption patterns.

## Project Structure
```
world-energy-consumption/
│
├── world_energy_consumption.csv   # Raw dataset
├── energy_app.py                  # Main Streamlit application
├── energy_model.pkl               # Trained ML model
├── energy_scaler.pkl              # Feature scaling object
├── column_names.pkl               # Saved column names for prediction
├── top_countries.pkl              # List of countries used in training
├── requirements.txt               # Project dependencies
└── README.md                      # Project documentation
```

## Features
- Predict primary energy consumption
- Interactive Streamlit web application
- Visualizations of energy consumption
- Feature importance analysis
- Simple and interpretable machine learning model

## Prerequisites

### System Requirements
- Python 3.8+
- Minimum 4GB RAM
- Internet connection for initial setup

### Required Libraries
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- streamlit
- joblib

## Installation Steps

1. Clone the repository:
```bash
git clone https://github.com/yourusername/world-energy-consumption-ml.git
cd world-energy-consumption-ml
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

3. Install required dependencies:
```bash
pip install -r requirements.txt
```

4. Download the dataset:
- Visit https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption
- Download `world_energy_consumption.csv`
- Place it in the project directory

## Running the Application

### Training the Model
```bash
streamlit run energy_app.py
```
1. Select "Train Model" from the sidebar
2. Click "Load Data and Train Model"
3. Observe model performance metrics and feature importance

### Making Predictions
1. After training, switch to "Make Predictions" mode
2. Select a country from the dropdown
3. Adjust input parameters using sliders
4. Click "Predict Energy Consumption"

## Model Details

### Algorithm
- Linear Regression
- Feature scaling with StandardScaler
- Top 20 countries used for training

### Performance Metrics
- Root Mean Squared Error (RMSE)
- R² Score
- Feature Importance Visualization

## Visualizations
- Pie chart of energy source distribution
- Bar chart of feature importances
- Comparison of input values with dataset averages

## Limitations
- Predicts based on historical data
- Limited to top 20 countries
- Simplified linear model
- Requires recent, clean dataset

## Potential Improvements
- Use more advanced algorithms (Random Forest, Gradient Boosting)
- Include more features
- Add time series analysis
- Implement cross-validation

## Troubleshooting
- Ensure all required libraries are installed
- Verify dataset is in the correct location
- Check Python version compatibility
- Retrain the model if prediction fails

## Contributing
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## Contact
Midhun J

## Acknowledgments
- Dataset source: Kaggle
- Libraries: pandas, scikit-learn, streamlit
- Inspiration: Global energy consumption research
