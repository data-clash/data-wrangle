# udacity-data-wrangle
Gather, Assess, clean and store data 

> Goal
Wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. The Twitter archive is great, but it only contains very basic tweet information. Additional gathering, then assessing and cleaning is required for "Wow!"-worthy analyses and visualizations.

> Data Description

1. The WeRateDogs Twitter archive. --> twitter_archive_enhanced.csv
The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, tweets are filtered with ratings only (there are 2356).Rating System > http://knowyourmeme.com/memes/theyre-good-dogs-brent

2. The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (image_predictions.tsv)
The results: a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).

3. Each tweet's retweet count and favorite ("like") count at minimum, and any additional data you find interesting. Using the tweet IDs in the WeRateDogs Twitter archive, query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Each tweet's JSON data should be written to its own line. Then read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count. 

> Data Assess 
Data is assessed programmatically and visually for quality and tidiness issues

> Data Cleaning 
The data is clean based on the results of the assessment 

> Data Storage
Finally the data is stored as a CSV file named twitter_archive_master.csv

> Results

1. wrangle_report.html briefly describes your wrangling efforts. This is to be framed as an internal document.
2. act_report.html communicates the insights and displays the visualization(s) produced from your wrangled data. This is to be framed as an external document, like a blog post or magazine article, for example.
