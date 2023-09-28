# Stock-Price-Prediction
The primary goal of this project is to create a simple and a basic stock market prediction model using Multiple linear regression.
In the real world, Stock market prediction is very complex, and it is a very challenging task as it is volatile and depends on numerous interrelated factors which makes it almost impossible to account for all the dependance factors. We have taken only a few significant features like open price, high price, low price, volume and created this model to 
predict our output, which is the close price. 
**Steps Involved **
1. Data Collection: We collected historical stock price data for the Microsoft company from 
yahoo finance source. This dataset includes stock prices data along with relevant features that 
could impact the stock prices from 2013-2023. 
2. Data Preprocessing: The data was checked for missing values, outliners and then divided into 
training and testing sets, with 80 percent of data used for training and 20 percent for testing. 
3. Linear Regression Algorithm: Multiple Linear regression algorithm is chosen due to its 
simplicity and interpretability. It assumes a linear relationship between the independent variables 
and the dependent variable. 
4. Model Training: The training data was used to train the linear regression model. During 
training, the model adjusted its weights and biases to minimize the difference between predicted 
and actual stock prices. 
5. Model Evaluation: The trained model was evaluated using the testing dataset. We used r2 
score metric to assess the model's performance. 
6. Model Prediction:  Once the model was trained and evaluated, we used it to predict stock 
prices for a specific day in the future. 
7. Model Visualization: After the model prediction is done, the data was visualized using 
Python’s matplotlib package which helped us to comprehend our model's performance. 
