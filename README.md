# ETH-LSTM
prediction of Ethereum by PyTorch LSTM using (fastquant) ETH and BTC dataset.

i use lstm with 2 layers and 100 nodes for each one.
1000 days of ETH and BTC data are fetched to train our model.
sklearn minmaxScaler has used to normalize dataset.
adam optimizer has used to optimize parameters
the learning rate i considered is 0.001
and model trained for 201 epoch ( last one is just for draw the plot and completion of 200 epochs )
i considered 2 step days sequence to predict 3th day. e.x first and second days data considered to predict 3th day close price.

at the end i have used FC layer to calculate and give me the 1 dimensional output.
