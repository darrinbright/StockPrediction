# Stock-Prediction-Using-LSTM
Stock price prediction involves analyzing historical stock price data with factors like economic conditions, company news, and market sentiments, thereby making the stock prices dynamic and volatile. While stock price prediction is challenging, advances in machine learning, like LSTM networks, show promise in improving accuracy.

The primary goal of this project is to create a Stock market prediction model using Long Short-Term Model(LSTM).

**IMPLEMENTATION OF LSTM**

1. **Importing the libraries**: Import the libraries mentioned into your python environment.
2. **Downloading Stock Price Data**: The Yahoo Finance library helps us in fetching historical stock price data from the start and end dates we specify.
3. **Normalizing the Data**: The closing prices are extracted from the dataset and reshaped. MinMaxScaler() is used to scale the data in the range of 0 and 1.
4. **Creating the input data**: LSTM models require the input data to be in a sequence format. This function takes a time series dataset and creates input-output pairs based on the specified time_steps. If the time_steps is 10, then for every sample, it will look at the last 10 samples to make a prediction.
5. **Reshaping of the data**: The data has to be reshaped into 3D format before feeding it to the LSTM model for it to be compatible with it. In the reshape function, the first parameter x.shape[0] is the number of samples, the second parameter x.shape[1] is the time steps, the last parameter is the number of features.
6. **Building the LSTM model**: This model comprises 2 LSTM layers and a Dense layer.
units refers to the number of neurons present in the specific layer. return_sequences=True is a must when we stack multiple LSTM layers as it ensures that the LSTM layers preserve the sequence information and pass it to the next layer.
7. **Regularization**: Dropout(0.2) is used to prevent overfitting by randomly setting a fraction of input units to zero during training of the model. BatchNormalization() is used to normalize the activations of each layer in a batch. It helps stabilize and speed up the training process by reducing the change in the distribution of layer inputs during training.
8. **Compiling the model**: "adam” is an adaptive learning rate optimization algorithm. "mean_squared_error” is a commonly used loss function for regression problems.
9. **Training the model**: 'epochs' refers to the iterations over the dataset to train the model. 'batch_size' refers to the number of samples to be processed in each iteration (batch) during training.
10. **Predicting the stock prices**: Test data is downloaded, and normalized, and input-output pairs are created for testing. The LSTM model is used to predict stock prices, and the predictions are inverse-transformed to get the original scale.
11. **Visualization**: To visualize the LSTM model’s performance, the actual and predicted stock prices are plotted using Matplotlib.
