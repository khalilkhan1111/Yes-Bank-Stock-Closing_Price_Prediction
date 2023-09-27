# Yes-Bank-Stock-Closing_Price_Prediction

The project focuses on analyzing the stock prices of Yes Bank, a prominent bank in the Indian financial sector, and predicting its monthly closing prices. The dataset used for this analysis, named "data_YesBank_StockPrices.csv," contains monthly stock price information since the bank's inception, including the opening, highest, lowest, and closing prices for each month. The project aims to determine if time series models or other predictive models can accurately predict stock prices, considering the impact of the fraud case involving Rana Kapoor, the bank's former CEO, which gained significant attention since 2018.

To begin the analysis, the dataset is explored to gain insights into the stock prices over time. A line graph is plotted to compare the closing prices from 2006 to 2020, providing a visual representation of the price fluctuations and trends. Additionally, scatter plots are used to examine the correlation between the dependent variable (closing price) and the independent variables (opening price, highest price, and lowest price). The scatter plots reveal a strong positive correlation between the dependent and independent variables.

To improve the predictions, the data is transformed using the logarithm base 10 (log10) function. This transformation aims to achieve a distribution that is closer to a normal distribution, as it is ideal for obtaining more accurate predictions. The independent variables (high, low, and open) are transformed using log10, as well as the dependent variable (close).

Next, feature handling techniques are employed to remove outliers from each column. Boxplots are utilized to identify and eliminate outliers that may adversely affect the accuracy of the predictive models.

Feature selection is carried out using Standard Scaler, Ridge regression. Cross-validation scores and average R2 scores are examined to determine the most appropriate features for the models.

To ensure the data is appropriately scaled, normalization is applied. This scaling technique ensures that all the features are on a similar scale, preventing any particular feature from dominating the model's predictions.

The dataset is then split into training and testing sets, with a test size of 20% and a train size of 80%. This division allows for the evaluation of the models' performance on unseen data.

Three machine learning algorithms are employed for prediction: Lasso regression, Ridge regression, and Elastic Net. These models are chosen for their effectiveness in handling regression tasks and their ability to provide reliable predictions. Each model is evaluated using cross-validation, which helps estimate the model's performance on unseen data.

By applying these techniques and models to the Yes Bank stock price dataset, the project aims to provide insights into the predictability of the bank's stock prices, considering the influence of the Rana Kapoor fraud case. The project assesses the effectiveness of time series models and other predictive models in capturing and predicting stock price movements. The ultimate goal is to generate accurate predictions that can assist investors and stakeholders in making informed decisions regarding Yes Bank stock.
