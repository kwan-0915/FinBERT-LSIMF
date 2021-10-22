# *FinBERT-SIMF* RESTFul API

This open source and free API available financial market data, financial News and financial market time series forecasting through a deep neural network model. Our predictive model jointly used news and public market data for financial decision support. 

- Please refer to [Postman documentation](https://documenter.getpostman.com/view/12212480/Tz5qZcaL) for visiting our API documentation.
- Please refer to this [Link](https://figshare.com/articles/dataset/MarketData_for_MarketPredict_RESTFul_API_including_News_and_Market_Data/14754966) for downloading our news and market datasets contains over 3 years of data.


For running this tools, you must install MongoDB at first and then the installation guide for each component of our tool is available in corresponding folder. Our tool containes three major components of MongoDB engines, News Scrapers and Prediction Services. Please refer to corresponding folder for more details.

Our FinBERT-SIMF tool works for price prediction in the FOREX and Cryptocurrency markets. For FOREX, we analysis
major currency pairs such as *EUR/USD*, *USD/JPY*, GBP/USD and for Cryptocurrency we focus on BTC/USDT.

###### Following figure shows the prediction plot of our model for major currency pairs in the FOREX market.

![EURUSD Prediction Plot](https://github.com/FinBERT-SIMF/FinBERT-SIMF/blob/ab8bd8af8429627dae83cb86ee643f4d8baf59d9/EURUSD_prediction.png)
<div align="center"><span style="color:blue">FinBERT-SIMF prediction plot of EURUSD during 6 month of test set.</span></div> 

![USDJPY Prediction Plot](https://github.com/FinBERT-SIMF/FinBERT-SIMF/blob/ab8bd8af8429627dae83cb86ee643f4d8baf59d9/USDJPY_prediction.png)
<div align="center"><span style="color:blue">FinBERT-SIMF prediction plot of USDJPY during 6 month of test set.</span></div>

![GBPUSD Prediction Plot](https://github.com/FinBERT-SIMF/FinBERT-SIMF/blob/ab8bd8af8429627dae83cb86ee643f4d8baf59d9/GBPUSD_prediction.png)
<div align="center"> <span style="color:blue">Prediction plot with FinBERT-SIMF for GBPUSD during 6 month of test set.</span></div>

###### We also analysis the amount of information gain of features and present the results in following table.

![Informaion gain and LSTM weights](https://github.com/FinBERT-SIMF/FinBERT-SIMF/blob/ab8bd8af8429627dae83cb86ee643f4d8baf59d9/L2_norm.png)

Information gain and L<sup>2</sup> norm of LSTM layer weights corresponding to each market and mood based features. Cells with * mark, negatively correlated with target close price of the corresponding market.

We implemented FinBERT-SIMF on top of MarketPredict tool available [here](https://github.com/MarketPredict-BoEC/MarketPredict-RESTFul-API). We preserve the architecture of MarketPredict and only implement our predictive model on top of it. 

Please visit following services : 
- news scraper services in newsscraper folder
- Model training Services in trainingServices folder
- Prediction Services in predictionServices folder
 

