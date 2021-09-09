**GameStop Stock Price Analysis and Prediction using LSTM**

Final Group Project for Graduate Level Machine Learning Course 

**Description**                                                               

We will use two datasets: 1st GameStop Historical Stock Price and 2nd Reddit Comments Datasets. Firstly, we have the GameStop (NYSE: GME) historical stock price updated through today. You’ll be able to visualize the growth of GME from their IPO until today (this dataset will be updated continually as new data is received). And second, we have a dataset containing each Reddit post from the WSB subreddit mentioning GME over the past month.
File names in drive: GME_Stock_History.csv and r_wallstreetbets_posts.csv

![image](https://user-images.githubusercontent.com/63076021/132599181-94ed279c-1a04-4e23-9c62-aba96c1364f1.png)

**Motivation**     

i.	We plan to determine future stock growth based on past comments because it seems that buyers are trying to push the stock price up to bet against hedge funds.                                             
ii.	Looking for potential correlation that could relate to the future stock price.                                    
iii.	Conduct sentimental analysis from Reddit comments text.
iv.	Predict GME stock price using GME stock history                                                      

**Installation**

For this project, you will need to make sure the following is installed:
i.	Tensorflow/Keras                                            
ii.	TextBlob                                               
iii.	Pandas
iv.	Scikit-learn                                              
v.	Matplotlib                                    

**Tools / methods** 

i.	Python 3 - Jupyter Notebook                                                     
ii.	Time Series Forecasting using LSTM (Open Stock Price)                                          
iii.	Text Analysis/Sentimental Analysis- using TextBlob using LSTM (Reddit comments converted to Sentimental value)

**Key findings**

![image](https://user-images.githubusercontent.com/63076021/132598846-d30352ea-f331-4e0f-9fe4-faec04a7ea41.png)
![image](https://user-images.githubusercontent.com/63076021/132598897-c33895be-4c84-40a3-b5e2-2551e627c9a0.png)

In conclusion, our results show that:                                                  
i.	Time Series Forecasting using LSTM to predict GME Open Stock Price, we use the first 60-day data to predict the 61st Open price, the predicted price is nearly same as real price, and performance metrics MSE (Mean Square Error) is acceptable (0.26).             
ii.	Bi-directional LSTM is better than unidirectional LSTM, our model indicated that MSE and MAE are both decreased compared with unidirectional LSTM.                                                    
iii.	We cannot say that the Reddit comments have influence on the stock price. From the output of LSTM model on TextBlob Sentimental Analysis on Reddit review comments, the predicted GME stock price nearly keeps unchanged.                                
iv.	Do reviews really have no effect on stock prices? Our LSTM model indicated it, but we only call TextBlob to get these comment’s Sentimental, Are they right? What’s more, we aggregate these sentimental value per-day, is it reasonable? Furtherly, review comments would mostly be affected by many factors, like country Policy on culture industry, company News and strategy, economy environment change like COVID. Besides these, we need look into more Natural Language processing work such as implementing an NLP transformer model for the Reddit data. In a word, we shall do more to get more confidential conclusion on whether review affect stock price.

**Authors and acknowledgment**

Project Team Members: Maxine M. Thao, TianXin Shao, Leon Tan, Pa Xiong Vang, Joseph D. Verbout

Special thanks for the following links for the data and information:
https://training.bielite.com/topic/gamestop-stock-and-reddit-datasets/
https://www.kaggle.com/gpreda/reddit-wallstreetsbets-posts/tasks 

