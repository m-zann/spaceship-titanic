# **Starship Titanic Project**

## Overview

The **Starship Titanic Project** is an exploratory data analysis and machine learning initiative aimed at predicting passenger survival on the fictional Starship Titanic, a space cruise liner. Inspired by the classic Titanic disaster, this project leverages a dataset containing various features related to passengers, such as demographics, travel details, and cabin information.

## Objectives

The primary objectives of the Starship Titanic Project are:

- **Data Exploration:** To analyze and visualize the dataset to uncover patterns and insights related to passenger survival.
- **Feature Engineering:** To create new features that may enhance the predictive power of the model.
- **Model Development:** To build and evaluate various machine learning models to predict the likelihood of a passenger's survival.
- **Hyperparameter Tuning:** To optimize model performance through systematic tuning of hyperparameters.
- **Model Evaluation:** To assess the effectiveness of the models using appropriate metrics and validation techniques.

## Dataset

The dataset includes the following variables:

- **PassengerId**: Unique identifier for each passenger.
- **HomePlanet**: The planet the passenger departed from.
- **CryoSleep**: Indicates whether the passenger elected to be put into suspended animation for the duration of the voyage.
- **Cabin**: The cabin number where the passenger is staying.
- **Destination**: The planet the passenger is traveling to.
- **Age**: Age of the passenger.
- **VIP**: Whether the passenger has paid for special VIP service during the voyage.
- **RoomService**: Amount the passenger has billed for room service.
- **FoodCourt**: Amount the passenger has billed at the food court.
- **ShoppingMall**: Amount the passenger has billed at the shopping mall.
- **Spa**: Amount the passenger has billed at the spa.
- **VRDeck**: Amount the passenger has billed at the VR deck.
- **Name**: The name of the passenger.
- **Transported**: Whether the passenger was transported to another dimension (target variable).

## Tools Used

- **Python**: The primary programming language used for the analysis.
- **Jupyter Notebook**: For coding, visualizing, and documenting the analysis process.
- **Numpy**: For mathematical operations.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib/Seaborn**: For data visualization.
- **Scikit-learn**: For machine learning and model evaluation.
- **Optuna**: For hyperparameter tuning.
- **SHAP**: For model interpretation.

## Key Findings

- **Imbalanced Data**: The dataset is relatively balanced with respect to the target variable, `Transported`.
- **Feature Engineering**: New features such as `GroupID`, `GroupSize`, `IsAlone`, `TotalExpenses`, and `CabinOrdinal` were created to enhance the predictive power of the model.
- **Model Selection**: Various models including Logistic Regression, Decision Tree, Random Forest, K-Nearest Neighbors, CatBoost, XGBoost, and LightGBM were evaluated.
- **Hyperparameter Tuning**: RandomizedSearchCV and Optuna were used for hyperparameter tuning to optimize model performance.
- **Model Evaluation**: The best-performing model achieved an accuracy of over 80%, combining the precision and recall results of different models. SHAP analysis provided valuable insights into how different features influence the model's predictions.

## How to Run the Analysis

To run the analysis, follow these steps:

1. Ensure you have Python installed on your machine.
2. Clone this repository to your local machine.
3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Open the Jupyter Notebook:

    ```bash
    jupyter notebook spaceship_titanic.ipynb
    ```

5. Run the cells sequentially to replicate the analysis.

