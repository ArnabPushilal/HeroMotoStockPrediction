# Table of Contents
* [Motivation](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#Motivation)
* [Data](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#Data)
* [Moving Average](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#moving-average)
  * [Moving Average + Window](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#moving-average--window)
  * [Moving Average + Difference to account for periodic data](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#moving-average--difference-to-account-for-periodic-data)
  * [Moving Average + Smoothening](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#moving-average--smoothening)
 * [DNN](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#DNN)
 * [LSTM](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#LSTM)
  * [LearningRate](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#LearningRate)
  * [Prediction](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#Predcition)
 * [Final Accuracy Table](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/README.md#final-accuracy-table)
 
 




## Motivation 
I wanted to explore time-series data predction from the stock prices of the company I work in.

### Data

![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/StockData.jpg)

It's about 20 years of data, I chose the closing price for prediction.

### Moving Average

 #### Moving Average + Window
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/movingaverage.jpg)
 
 We can see this just smoothenes out the data, large errors are still present
 
 #### Moving Average + Difference to account for periodic data
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/Differnce%20Series%20for%20Periodical%20data.jpg)
 
 * Some data might be dependant on Quarter results, so I chose a period of 90 days to see if it improved my model.
 #### Moving Average + Smoothening
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/Moving%20Average%20Plus%20Period.jpg)
 
 * This looks better!
 
 ### DNN
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/DenseNetworkPrediction.jpg)
 
 
 ### LSTM
 
  ### LearningRate
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/learningrate%20(4).jpg)
 5e-5 seems to be the best choice
 
  ### Prediction
  

 ### Final Accuracy Table
  
 
 
