
1. Project Title.
GameStop Stock Price Analysis, and Prediction using LSTM
2. Description of data source and web link(s).
We will use two datasets: 1st GameStop Historical Stock Price and 2nd Reddit Comments Datasets. Firstly, we have the GameStop (NYSE: GME) historical stock price updated through today. You’ll be able to visualize the growth of GME from their IPO until today (this dataset will be updated continually as new data is received). And second, we have a dataset containing each Reddit post from the WSB subreddit mentioning GME over the past month.
File names in drive: GME_Stock_History.csv and r_wallstreetbets_posts.csv
Special thanks for the following links for the data and information (data can also be found on the first link below):
https://training.bielite.com/topic/gamestop-stock-and-reddit-datasets/
https://www.kaggle.com/gpreda/reddit-wallstreetsbets-posts/tasks 
3. # of records & # of attributes with description of each attribute.
Size of Dataset
Records: 884,640 (raw data) As of March 14th, 2021, there are 884,640 of records in the dataset. We have chosen to filter out any blanks, unknown, NA values. Also, removing columns such as dividends and stock splits since GameStop have not reach that financial stage.
Number of Attributes
This dataset (after merging) has 16 attributes. Below attributes Index 1 – 6 are from 1st dataset, 7-16 are from 2nd dataset. 
Description of Attributes
Index	Name	Description	Type
1	Date	The date when the prices were recorded	Date
2	Open	The stock price at market open	Decimal
3	Close	The stock price at market close	Decimal
4	Low	The lowest stock price recorded during the trading period	Decimal
5	High	The highest stock price recorded during the trading period	Decimal
6	Volume	The total number of shares traded during the trading period	Integer
7	Id	The reddit post id	Integer
8	Title	The title of the Reddit post	String
9	Score	The score of the reddit post (upvotes – downvotes).	Decimal
10	Author	Author of the post	String
11	author_flair_text	Describes is the author has any flair (self-chosen tag)	Text
12	removed_by	Describes who the post was removed by, if anyone	String
13	total_awards	The number of awards the post received	Integer
14	awarders	Who provided the rewards	String
15	created_utc	The UTC timestamp when the post was created	Date
16	num_comments	The total number of comments for the post	Integer

4. Some general statistics of the dataset.
Among 884,640 records, GME was mentioned 61,284 times and GameStop was mentioned 6,852 times in the “title” attributes.
The all-time high GME stock closing price was 347.51 on Jan 27,2021
The 52-week high for GME is ~$483, and 52-year low is ~$2. 
The average GME stock price for the last 52 weeks is $25.29
5. Tools / methods your team (plan to) use in your study.
i.	Python- Jupyter Notebook
ii.	Time Series Forecasting using LSTM (Open Stock Price)
iii.	Text Analysis/Sentimental Analysis- using TextBlob using LSTM (Reddit comments converted to Sentimental value)
6. Detail description of what problems/questions your team plans to predict / study.
i.	We plan to determine future stock growth based on past comments because it seems that buyers are trying to push the stock price up to bet against hedge funds. 
ii.	Looking for potential correlation that could relate to the future stock price. 
iii.	Conduct sentimental analysis from Reddit comments text.
iv.	Predict GME stock price using GME stock history
7. Conclusions
In conclusion, our results shows that we cannot say that the Reddit comments have influence on the stock price. From our project we found that stock prediction is difficult to due to various economic and stock price-related indicators. In addition to that, public review comments of stock might be misleading because we could not determine if the price could affect by the comments.  However, in order to improve our dataset, we could collect more Reddit review data to combine with Stock Dataset. We can set up PRAW to scrape reddit data. In addition, we could have looked more into getting more GME Stock Data and looking into more factors that impacts Stock price, like policy, news, industry, etc. As well as looking into more Natural Language processing work such as implementing an NLP transformer model for the Reddit data. An example of a transformer model that is popular right now is the BERT model.  


