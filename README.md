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

![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/StockData.jpg)

It's about 20 years of data, I chose the closing price for prediction.

## Moving Average

 ### Moving Average + Window
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/MovingAvg.jpg)
 
 We can see this just smoothenes out the data, large errors are still present
 
 ###  Difference series to account for periodic data
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/DifferenceSeries.jpg)
 
 * Some data might be dependant on Quarter results, so I chose a period of 90 days to see if it improved my model.
 ### Moving Average + Difference 
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/MovingAvgpluspast.jpg)
 
 ### Moving Average + Difference + Smoothening
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/MovingAvgSmooth.jpg)
 
 ## DNN
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/DenseNetwork.jpg)
 
 
 ## LSTM
 
  ### Picking LearningRate
  
 ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/LearningRate%20(2).jpg)
   
 
 
  ### Prediction
  ![](https://github.com/ArnabPushilal/HeroMotoStockPrediction/blob/main/images/LSTM.jpg)

 ## Final Accuracy Table
  
 |Model |MSE| MAE |
|--- | --- | --- |
| Moving Average | 32488.284 | 143.392 |
| Difference Series |  50870.056|180.291|
| Moving Average + Difference + Smoothening|  37266.263 | 156.276|
| Dense Network | 11013.445 | 82.419 |
| LSTM | 10364.572| 80.46758|



 
