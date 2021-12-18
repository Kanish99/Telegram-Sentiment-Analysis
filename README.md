# Telegram-Sentiment-Analysis

### How to run the code
 1. Run the requirements.txt file using command
    $ pip install -r requirements.txt
 2. Open the .ipynb python file in Jupyter Notebook(Ananconda) or Google Colab
    2.1 If you are using Jupyter Notebook then just open file from Downloads and start running the cells as the json file will be in the same path as that of the file.
    2.2 If you are Google colab then you need to upload the result.json file in to its environment. Once it gets uploaded then just simply run the cells and you will get the desired output. 


### Flow and Explanation of Code
    1. Initially we began with making function for removing emojis and converting the emoticons to their literal meaning.
    2. Then we focus on pre-processing the text such as removing unnecessary words and non-English messages, lower capital case conversion. Also, the date was converted to number of days for making the plotting easy and convinient.
    3. In the 2nd section itself I applied the condition of using only messages consisting of Doge or Shib words and displaying only those records in the dataframe. 
    4. In the 2nd and 3rd combined section I applied tqdm package to display the progress of code on the terminal.
    5. Implementing the textblob NLP pre-trained model. Due to time constraint I didn't implemented my own model and took TextBlob for finding out the sentiment polarity and it was giving good polarity. I also tried other pre-trained models but was not satisfied with the sentiment polarity.
    6. In the 5th point itself a new dataframe was created named sentiment which would categorise each text message in to positive, negative and neutral sentiments.
    7. At the end plotly was used for visualization purpose to plot the Number of days vs Average sentiments made per day and the graph is obtained which can be seen in the code as well as the screenshot attached.


### Summary of Results
    The graph obtained for the Number of days vs Average Sentiment per day depicted that on a particular day how many text were classified and that to what was the sentiment behind that text. Like for instance talking about the 10th day 471 text messages were classified as having Neutral sentiment, 160 messages for positive snetiment and 89 messages for negative sentiment by the textblob pre-trained model. In this way sentiment analysis was carried out from May 1 to May 15 and with the necessary conditions included I got this sentiment analysis for the messages. 


