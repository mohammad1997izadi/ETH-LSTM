# ETH-LSTM
Ethereum Price Prediction Using PyTorch LSTM with Fastquant ETH and BTC Dataset

This project uses a Long Short-Term Memory (LSTM) network implemented in PyTorch to predict Ethereum prices, leveraging the ETH and BTC dataset provided by Fastquant.

The model architecture consists of two LSTM layers, each with 100 hidden units. A total of 1,000 days of historical data for both ETH and BTC is used to train the model. Prior to training, the dataset is normalized using sklearn’s MinMaxScaler.

The Adam optimizer is used to update the model parameters, with a learning rate set to 0.001. Training is conducted over 201 epochs—the final epoch serves solely to generate the output plot and complete the 200 training cycles.

The model is designed to use a two-day sequence of data to predict the closing price on the third day. For example, data from day one and day two are used to predict the closing price for day three.

Model parameters can be saved after training. If saved parameters are available, the training phase can be skipped. A fully connected (FC) layer is used at the end to produce a single-dimensional output representing the predicted price.
