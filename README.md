# HDFC-BANK-Stock-Price-Prediction

The Stock Price Prediction Project aims to develop and evaluate a predictive model for anticipating stock price movements within a 2-4 week horizon, specifically focusing on the 'HDFC Bank' stock. The project utilizes historical data sourced from Yahoo Finance, with the primary goal of providing swing traders with precise insights into opportune entry and exit points for their positions.

Objectives

Develop Predictive Model:

Create a predictive model utilizing polynomial regression and the AutoRegressive Integrated Moving Average (ARIMA) model.

Empower Swing Traders: 

Provide swing traders with accurate insights into entry and exit points for positions in the 'HDFC Bank' stock.

Utilize Historical Data: Utilize historical stock price data from Yahoo Finance until the specified date (2023-12-02).

Methodology

Data Exploration

Data Source: Utilized the yfinance library for its well-maintained, structured, and easily usable historical data.

Data Cleaning: 

Since data was already clean, minimal cleaning was required. Visualized the adjusted closing price of the stock, revealing an overall increasing trend over time.

Time Horizon Analysis: 

Histogram analysis suggested that a time horizon of 2-4 weeks is suitable for earning good returns.

Correlation Analysis: 

Correlation heatmap showed high correlation among Open, High, Low, Close, and Adjusted Closing prices, while all these variables weakly correlate with trading volume.

Efficient Market Hypothesis: 

Rejected the Efficient Market Hypothesis based on a low p-value (0.00042), suggesting the possibility of predicting future prices using historical prices for stocks.

Model Development

Dataset Splitting: 

Split the dataset into 80% for training the machine learning model and 20% for validation.

Polynomial Regression: 

Experimented with polynomial regression of the 7th degree, yielding an RMSE of approximately 170 but found not suitable for capturing time series data.

ARIMA Model: 

Explored the ARIMA model with an order of (5, 2, 2), capturing autoregressive, differencing, and moving average components.

Model Evaluation: 

Evaluated both models based on their respective RMSE values. Polynomial regression had an RMSE of 170, while the ARIMA model achieved an improved RMSE of 117.

Model Refinement

Refinement: 

Conducted model refinement, potentially through manual experimentation, leading to an improved RMSE value for the ARIMA model.

Future Predictions: 

Developed a methodology for making future predictions using the ARIMA model, achieving an accuracy of 90-93%.

Recommendations and Next Steps

Continuous Monitoring: Implement continuous monitoring and evaluation of the ARIMA model's performance, updating it regularly with new data.

Exploration of Advanced Models: 

Consider exploring alternative time series forecasting models or ensemble methods to further enhance predictive capabilities.

Outcome

The project highlights the significance of model selection and iterative refinement. The ARIMA model emerged as the preferred choice for stock price prediction in this context, achieving a higher accuracy level compared to polynomial regression. Continuous monitoring, regular updates, and exploration of additional features are recommended for maintaining and enhancing the model's accuracy over time. The accuracy achieved (90-93%) positions the model as a valuable tool for swing traders seeking precise insights into 'HDFC Bank' stock movements.
