# semester_project


## The intended order of viewing files:

**1. Bibliometric analysis (bibliometrics_record_collections_final)**

*This file is disconnected from the rest of the pipeline, it's just the analysis of our search string for the projects literature review*


to do: 

- clen up the networks

- comments


**2. Getting financial data and exploratory analysis (NASDAQ_100_exploration_UML)**

*In this notebook we're downloading yf data and conducting exploratory analysis based on which a set of companies to be used for SML is chosen. At the end of the file a dataset with all the needed data for selected companies is exported.*


**3. Twitter scraper (twitter_scraper)**

*This code was run in the visual studio code console to scrape the tweets for the four companies chosen in the previous notebook*


**4. Title scraper (title_scraper)**

*This code was run in visual studio code, because scraping of the smallest dataset took around 20h. It actually is still being run (since the 23rd december) on two computers for two datasets - sadly, the number of tweets for those companies is very high, so we're not 100% sure if it will finish on time. In hindsight, we probably should have chosen companies that aren't talked about as much.*


**5. Supervised ml without text data (improved_deep_learning_of_uml+deeplearning)**

*This notebook uses the data acquired in notebook 2 to do random forest regression, linear regression and a simple neural network for stock predictions*
    


**6. Supervised ml with text data (ml models for stock data and titles)**

*The notebook using stock data and the scraped headlines for stock prediction*


to do: 

- comments


**7. Backtesting (no file shared yet - we're working on it)**


to do: 

- everything



## Contents of the data folder:

**- ticker_data.zip** - the databases with the tweets about the three chosen companies (out of four - the tesla one was too big even after zipping, we will figure out a way to provide it if it will be used in code)

**- proc_ticker_data.csv** - the databases containing headlines of news articles for the chosen companies (so far only alexion)

**- raw_partner_headlines.csv.zip** - a very large dataset containing many financial news titles, we're using it for training the embedding layer (to avoid fitting it specifically to our data). Source: https://www.kaggle.com/miguelaenlle/massive-stock-news-analysis-db-for-nlpbacktests

**- sentiment_data.csv** - dataset for training a sentiment model. Source: https://www.kaggle.com/ankurzing/sentiment-analysis-for-financial-news

**- yf_chosen_comp.csv** - the dataset created in the notebook from point 2. Contains daily closing information for the chosen companies.
