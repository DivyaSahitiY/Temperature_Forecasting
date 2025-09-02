## Project Overview
This project demonstrates a time series forecasting model using a Long Short-Term Memory (LSTM) neural network. The goal is to predict future climate conditions, specifically temperature, based on historical data. To evaluate the performance of the LSTM model, it is compared against a baseline model - Seasonal Naive.
## Dataset
The model uses the Jena Climate Dataset, which is available on [Kaggle](https://www.kaggle.com/datasets/mnassrib/jena-climate). It contains various climate features recorded every 10 minutes from 2009 to 2017. The dataset includes features such as temperature, pressure, humidity, and wind speed. For this project, the data is preprocessed to be hourly.
## Technologies and Libraries
The project is built with Python and utilizes the following key libraries:

TensorFlow: For building and training the LSTM model.

Pandas: For data manipulation and analysis.

NumPy: For numerical operations.

Matplotlib: For data visualization, including plotting the predictions against actual values.

Scikit-learn: For data preprocessing, including scaling, and evaluation metrics like Mean Absolute Error (MAE).

## Model Training and Evaluation
Data Preprocessing: The dataset is cleaned and normalized using StandardScaler from scikit-learn to prepare it for the neural network. The data is split into training and testing sets.

Model Architecture: A sequential LSTM model is constructed. The model consists of two LSTM layers, followed by dense layers to output the predictions.

Training: The model is trained using the Adam optimizer and MeanSquaredError as the loss function.

Prediction: The trained model is used to make predictions on the test set.

Evaluation: The performance is evaluated using the Mean Absolute Error (MAE) metric, which is also used to establish a baseline for comparison. The model's predictions are also visualized against the actual values to assess its performance.
## How to Run
Clone the repository.

Install the required libraries:

```pip install tensorflow pandas numpy matplotlib scikit-learn```

Ensure the jena_climate_dataset.csv file is in the same directory as the notebook.

Open and run the LSTM_Time_Series_Forecasting.ipynb notebook.
