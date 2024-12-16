

# Predicting Quality of Service (QoS) in Vehicular Networks

## Overview
This project focuses on predicting **Quality of Service (QoS)** metrics, such as **downlink throughput**, in vehicular networks using **machine learning models**. Leveraging the **XGBoost** algorithm and real-world datasets, the project aims to improve communication reliability in dynamic vehicular environments.

---

## Project Structure

- **`xgboost_networking_project.ipynb`**  
   Contains the implementation of the XGBoost model for QoS prediction. It includes:
   - Data preprocessing (feature encoding, normalization, and selection)
   - Model training and testing
   - Performance evaluation using key metrics
   - Visualizations of residuals and predictions

- **`Train.csv`**  
   Training dataset with features and target values for model development.

- **`Test.csv`**  
   Testing dataset for evaluating the model's performance.

- **`SampleSubmission.csv`**  
   Submission template for predictions formatted similar to the test dataset.

- **`VariableDefinitions.csv`**  
   A file describing the dataset features.

- **`README.md`**  
   Documentation and project overview.

---

## Dataset Description

The dataset consists of key features critical for predicting **downlink throughput**:
- **Signal Metrics**  
   - SINR, RSRP, RSRQ, and resource block usage  
- **Environmental Data**  
   - Location (latitude, longitude), speed, and area types (e.g., residential, park)  
- **Timestamp**  
   - Used for splitting data into realistic training and testing subsets  

The training and testing datasets simulate real-world conditions, enabling robust evaluation of the predictive model.

---

## Implementation Details

### Machine Learning Model
- **XGBoost** (Extreme Gradient Boosting): A tree-based ensemble method for handling tabular data.
- **Evaluation Metrics**:  
  - Mean Squared Error (MSE)  
  - Root Mean Squared Error (RMSE)  
  - Mean Absolute Percentage Error (MAPE)  
  - Coefficient of Determination (R²)  

### Data Preprocessing
- Encoding categorical variables (e.g., area type, operator, device ID)  
- Normalizing continuous features (e.g., SINR, RSRP)  
- Handling missing values  
- Splitting training and testing data based on timestamps  

### Visualizations
- **Residual Plots**: Analyze the error distribution between predicted and actual values.  
- **Actual vs Predicted Curves**: Visualize the model’s accuracy in predicting downlink throughput.  

---

## How to Run

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/qos-prediction.git
   cd qos-prediction
