# 2024-P6-CYF (Corn Yield Prediction Project)
This project focuses on predicting **Fresh Ear Yield** and **Dry Ear Yield** of corn using various machine learning models and advanced feature engineering. The dataset includes meteorological variables and corn yield data collected over multiple years. The project applies preprocessing, feature engineering, exploratory data analysis, and multiple regression techniques to develop accurate predictive models.<br/>
<br/>


## Table of Contents

1. [Overview](#overview) 
2. [Datasets](#datasets)
3. [Project Workflow](#project-workflow)
   - Stage 1: Data Preprocessing & Feature Engineering
   - Stage 2: Train-Test Split
   - Stage 3: Exploratory Data Analysis (EDA)
   - Stage 4: Normalization
   - Stage 5: Model Training and Evaluation
4. [Models Used](#models-used)
5. [Performance Metrics](#performance-metrics)
6. [Visualizations](#visualizations)
7. [How to Use](#how-to-use)
8. [Dependencies](#dependencies)
9. [Results](#results)
10. [Contributors](#contributors)
<br/>


## Overview

The goal of this project is to predict corn yields based on meteorological and crop-related features. A variety of machine learning models are trained and evaluated to determine the best performance on two targets:
- **Fresh Ear Yield**: Predicted yield of fresh corn ears.
- **Dry Ear Yield**: Predicted yield of dried corn ears.

The project pipeline involves:
- Data merging and preprocessing.
- Handling missing values and scaling.
<br/>


## Datasets

1. **`meteo_variables.csv`**: Meteorological variables such as temperature, precipitation, humidity, and wind speed.
2. **`meteo_station.csv`**: Station-level meteorological data with daily records.
3. **`corn_yield.csv`**: Corn yield data with information on crop variety, fresh and dry yield, and ear percentages.
<br/>


## Project Workflow

### Stage 1: Data Preprocessing & Feature Engineering
- Merge datasets based on year and handle missing values .
- Engineer features for monthly meteorological statistics from March to October.

### Stage 2: Train-Test Split
- Split the dataset into training (2012-2020) and test (2021-2023) sets.

### Stage 3: Exploratory Data Analysis (EDA)
- Visualize distributions, relationships, and correlations between features and targets.

### Stage 4: Normalization
- Normalize features using **MinMaxScaler** for consistent scaling.

### Stage 5: Model Training and Evaluation
- Train models (e.g., Random Forest, XGBoost, Ridge, etc.) and evaluate them using various metrics.

<br/>

## Models Used

1. **Random Forest**: Default and tuned models using Grid Search.
2. **XGBoost**: Boosted decision tree model.
3. **Linear Models**:
   - Ridge
   - Lasso
   - ElasticNet
4. **Gradient Boosting Regressor**: Gradient-based optimization.

<br/>

## Performance Metrics

Evaluate models with:
- **Mean Absolute Error (MAE)**.
- **Mean Absolute Percentage Error (MAPE)**.

<br/>

## Visualizations

1. **Feature Correlations**: Heatmaps of relationships between features and yields.
   <br/>
    ![5](https://github.com/user-attachments/assets/2ed0165a-a987-44e2-8549-9ebe5c32ce92)

<br/>

2. **Model Performance**: Bar charts comparing error metrics.
   <br/>
   ![1](https://github.com/user-attachments/assets/7cebff78-c9da-4904-b5b0-f78f2ba9ca77)
    ![2](https://github.com/user-attachments/assets/73384d10-2e0b-486a-ad70-3ad5c1e61b0e)
    ![3](https://github.com/user-attachments/assets/1bba02fd-171c-41e4-9c77-3d2bd30cd3c5)
    ![4](https://github.com/user-attachments/assets/00a5ff0d-9757-4243-82e0-dc18cc6f2a4e)
   <br/>
   <br/>
   
3. **Prediction Accuracy**: Scatterplots of actual vs. predicted values.
   <br/>
   ![6](https://github.com/user-attachments/assets/e1404e21-dcc8-4eb7-85fd-c4994acba565)

<br/>

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/corn-yield-prediction.git
   cd corn-yield-prediction

2. Install dependencies:
   ```bash
   pip install -r requirements.txt

3. Run the project:
   - Ensure the datasets are in the root directory.
   - Execute the notebook or script for each stage.

4. Use saved models for predictions:
   - Random Forest models are saved as **`.pkl`** files in the repository.
<br/>

 ## Dependencies

- Python 3.8+
- Libraries:
   - **`pandas`**
   - **`numpy`**
   - **`matplotlib`**
   - **`seaborn`**
   - **`sklearn`**
   - **`xgboost`**
   - **`joblib`**
   - **`missingno`**
 <br/>

## Results

- **Best Model**: Random Forest with Grid Search (Reduced Features).
- **Performance Highlights**:
  - Fresh Ear Yield MAE: 2.87 
  - Dry Ear Yield MAE: 1.84   
  - Fresh Ear Yield MAPE: 12.21%
  - Dry Ear Yield MAPE: 13.57%
  <br/>

## Contributors

- **Hamed Goldoust**
- **Parsa Taati**
- **Afsoun Abbasi**
