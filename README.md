# Data-scrapeing
# Problem Statement:
Today, data is scattered everywhere in the world. Especially in social media, there may be a big quantity of data on Facebook, Instagram, Youtube, Twitter, etc. This consists of pictures and films on Youtube and Instagram as compared to Facebook and Twitter. To get the real facts on Twitter, you want to scrape the data from Twitter. You Need to Scrape the data like (date, id, url, tweet content, user,reply count, retweet count,language, source, like count etc) from twitter.

# Approach:
By using the “snscrape” Library, Scrape the twitter data from Twitter Reference Create a dataframe with date, id, url, tweet content, user,reply count, retweet count,language, source, like count. Store each collection of data into a document into Mongodb along with the hashtag or key word we use to Scrape from twitter.

example:

({“Scraped Word”           : “Elon Musk”,

 “Scraped Date”            : 15-02-2023,
 
 “Scraped Data”            : [{1000  Scraped data from past 100 days }]})
 
Create a GUI using streamlit that should contain the feature to enter the keyword or Hashtag to be searched, select the date range and limit the tweet count need to be scraped. After scraping, the data needs to be displayed in the page and need a button to upload the data into Database and download the data into csv and json format.

# Results:

You have to build a solution that should be able to scrape the twitter data and store that in the database and allow the user to download the data with multiple data formats.
Workflow:
The code first inputs the Hashtag/Keyword from the user along with Date search range and limit of number of data.
The code then scrapes the data from Twitter and stores them in an array.
This array is then converted to a DataFrame and displayed on the screen.
The DataFrame is then converted to CSV and JSON formats along with eshtablising a connection with MongoDB Database for uploading purposes.
If the user clicks on Download options for each of the two data formats, the information gets downloaded in the desired file format.
User is then presented with an option of uploading the Data into the Database as initialized in step 4.
The code also creates a sidebar which shows all the uploaded Databases along with an option to delete all Databases.
Once the User clicks on a previously uploaded database, they are shown the data in a DataFrame format.
Additionally, the User is also presented with an option to download the old data in CSV and JSON format.

# Concepts involved:

 1.Python Scripting
 
 2.MongoDB
 
 3.Streamlit
 
 4.Snscrape
 
# HOW TO RUN TWITTER SCRAPER IN YOUR SYSTEM:
Pre-requisites: Python and MongoDB must be installed in your system.

Open cmd:

(base) C:\Users\Usernme>pip install virtualenv

(base) C:\Users\Usernme>virtualenv test_env

(base) C:\Users\Usernme>cd test_env

(base) C:\Users\Usernme\test_env>cd Scripts

(base) C:\Users\Usernme\test_env\Scripts>activate

(test_env) C:\Users\Usernme\test_env\Scripts>mkdir Scraper

(test_env) C:\Users\Usernme\test_env\Scripts>cd Scraper

At this point, download the github files into the folder created by step 7. This folder is most likely located in Users>Username>test_env>Scripts>Scraper. You can search for this folder by typing "Scraper" in the "Search this PC" tab in "This PC".

(test_env) C:\Users\Usernme\test_env\Scripts\Scraper>pip install -r requirement.txt

(test_env) C:\Users\Usernme\test_env\Scripts\Scraper>streamlit run Twitter_scrapping_code.py

You can now view your Streamlit app in your browser with URL : http://192.168.1.6:8501
