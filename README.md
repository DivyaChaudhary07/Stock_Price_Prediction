# StockFutura

## Objective:
The goal of the project is to predict the next day's stock price by training a machine learning model using historical stock data. The project likely uses 60 days of past stock price data as inputs to predict the price for the following day.

## Data Preprocessing:
The dataset includes stock price data like Open, High, Low, Close, and Volume. It could also include date/time columns.
Normalization/Scaling: Since stock prices can vary significantly, the data may be normalized or scaled, commonly using Min-Max scaling, to bring all features within a specific range.
Training Data: A sliding window of 60 days of past stock prices is used as input features, with the target being the price for the next day.

## Model Selection:
The project likely utilizes deep learning or time series-based models like LSTM (Long Short-Term Memory) or GRU (Gated Recurrent Unit). These models are widely used for time-dependent data like stock prices due to their ability to remember long-term dependencies.
The architecture of the model would likely include layers of LSTM or GRU units followed by dense (fully connected) layers to make the final prediction.

## Training:
The model is trained on a time-series format dataset, where each 60-day window is used to predict the stock price on the 61st day.
Train-Test Split: The dataset might be split into training and testing sets to evaluate model performance. The training set is used to learn patterns, while the testing set assesses the model’s generalization ability.
The loss function for stock price prediction is likely Mean Squared Error (MSE), which penalizes the differences between predicted and actual stock prices.

## Evaluation Metrics:
The model is evaluated using metrics such as MSE or Mean Absolute Error (MAE), which measure how close the predicted prices are to the actual prices.

|Mean Absolute Error (MAE) : 2.7980 😃📈|
|-|

## Results:
The model’s predictions are compared with actual stock prices for the test set. Visualizations such as line plots could be generated to compare predicted prices vs. real prices over time, illustrating the model's performance.

| ![download](https://github.com/user-attachments/assets/97bf8ef7-911e-41a0-a10d-4f4330ed0111) | ![download](https://github.com/user-attachments/assets/e0eee574-502a-4f38-aa2a-86cfad2448f8) |
|-|-|
| ![download](https://github.com/user-attachments/assets/f3b83985-9f67-4d9c-b948-930b94f6f5af) | ![download](https://github.com/user-attachments/assets/a4186d78-d038-4ae0-afd0-0b31c0173e77) |
| ![download](https://github.com/user-attachments/assets/e62a283e-40ce-4886-9327-e983f2e53159) | ![download](https://github.com/user-attachments/assets/ce6e7b16-42ea-4d10-9283-733b5a4dc7e0) |
| ![download](https://github.com/user-attachments/assets/c33ba27b-e3af-49c8-93dc-372feca5a494) | ![download](https://github.com/user-attachments/assets/036e1e14-6bbd-4925-ad18-15e3c718ccc4) |
