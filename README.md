# scrapping_and_sentiment_analysis_little_practice
 trying to do some sentiment analysis from some scrapped data

For this project, we will be scrapping some comments from a web page first. Then, once we have all the reviews, we will use them to practice some sentiment analysis.

# SCRAPPING THE DATA
We have all the code related to this scrapping process in "scrapy.ipynb". We use the [Selenium library](https://selenium-python.readthedocs.io/). We use this library because the web page we have use loads it content dinamycally. We have also used [BeautifulSoup](https://pypi.org/project/beautifulsoup4/) to deal with the parsig and the extraction of data.
Finally, we save the extracted data in a csv with:
- Review: number of the review
- Title: title of the review
- Content: the text of the review


# SENTIMENT ANALYSIS
In "sentiment_analysis.ipynb", we have all the work we have done for the sentiment analysis. We start by prepocessing the text, we then look for the sentiment score of each review, and we plot a WordCloud to help visualize the possitive and negattive words. Finally, we use TF-IDF. 

## TF-IDF
Term Frequency-Inverse Document Frequency is a way to measeure how important a word is in a document compared to other documents. It starts by counting how often a word appears in one document. It downweight words that appear too often everywhere. If a word is frequent in one document, but rare in others, it gets a high score.
