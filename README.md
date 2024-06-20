# Stock_Prediction_using_LSTM

NVIDIA Stock price prediction using the LSTM Model.
data source = Yahoo Finance --> https://finance.yahoo.com/quote/NVDA/history/

NVIDIA Stock has been showing huge returns in the 2023-2024 duration. The model trains the 2023-2024 data to forecast the data over the upcoming years.

## Model Construction
Step 1: Import libraries
Step 2: Loading dataset and plot the daily closing value
Step 3: Calculate the returns per day and plot the Log Return with mean and errors
Step 4: Create a windowed dataset such that the stock closing price of a day depends on the closing price of the previous three days. The model will find a closing price pattern with the three previous day's closing data.
Step 5: Reduce the data set to last one year. From 2023 May to 2024 May, there were 253 trading days.
Step 6: Devide the whole dataset into - training(80%), validation(10%), and testing(10%)
Step 7: Build a deep-learning LSTM model with 5 layers (input, 3 hidden layers, output). The neuron count and layer count are arbitrary. Choose the parameters according to the data.
Step 8: Compile the model with loss function as mean squared error (mse), Adam optimizer with arbitrary learning rate, and mean absolute error metrics
Step 9: Fit the model in the training data. Also, add the validation data as well. 
Step 10: Adjuct the epoch value according to achieve minimum mean absolute error on validation data. 
Step 11: Plot the train, validation, and text data with respect to date.
