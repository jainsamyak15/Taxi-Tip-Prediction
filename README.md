# Taxi Tip Prediction using Scikit-Learn and Snap ML

This project focuses on building a machine learning model to predict the tip amount for taxi trips in New York City using the Scikit-Learn and Snap ML libraries. The dataset used for this project is the NYC Yellow Taxi Trip Records of June 2019, provided by the Taxi & Limousine Commission (TLC), City of New York.

## Objective
The main objective of this project is to train a regression model to predict the tip amount paid for taxi trips based on various features such as pickup and dropoff locations, trip duration, payment type, and more.

## Libraries Used
- Scikit-Learn: Used for data preprocessing, model building, and evaluation.
- Snap ML: Utilized for accelerating the training of machine learning models, providing highly-efficient CPU/GPU implementations of linear and tree-based models.

## Dataset
The dataset contains information about taxi trips, including pick-up and drop-off dates/times, locations, payment types, and tip amounts. Before training the model, the dataset undergoes preprocessing steps such as removing outliers, converting datetime columns, extracting features, and encoding categorical variables.

## Model Building
### 1. Decision Tree Regressor with Scikit-Learn
- A Decision Tree Regressor model is built using Scikit-Learn, with hyperparameters tuned for optimal performance.
- The model is trained on the preprocessed dataset, and its training time and Mean Squared Error (MSE) on the test dataset are evaluated.

### 2. Decision Tree Regressor with Snap ML
- Another Decision Tree Regressor model is constructed using Snap ML, aiming for faster training.
- Snap ML offers multi-threaded CPU/GPU training and provides a seamless integration with Scikit-Learn APIs.
- The model is trained with the same hyperparameters as the Scikit-Learn model, and its training time and MSE on the test dataset are compared to the Scikit-Learn model.

## Results
- Both the Scikit-Learn and Snap ML Decision Tree Regressor models achieve comparable performance in terms of MSE on the test dataset.
- However, Snap ML demonstrates faster training time compared to Scikit-Learn, showcasing the advantage of using Snap ML for accelerating classical machine learning models.

## Project Structure
- `taxi_tip_prediction.ipynb`: Jupyter Notebook containing the code for data preprocessing, model building, and evaluation.
- `yellow_tripdata_2019-06.csv`: Dataset file containing the NYC Yellow Taxi Trip Records of June 2019.

## Instructions
1. Clone the repository: `git clone https://github.com/jainsamyak15/taxi_tip_prediction.git`
2. Navigate to the project directory: `cd taxi_tip_prediction`
3. Install the required libraries: `pip install -r requirements.txt`
4. Open and run the `taxi_tip_prediction.ipynb` notebook to explore the code and results.

