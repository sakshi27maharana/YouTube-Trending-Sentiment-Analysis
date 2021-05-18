# Trending YouTube Video Statistics
##### : Daily statistics for trending YouTube videos (2017-18) ------ by Sakshi Maharana

### Context
YouTube (the world-famous video sharing website) maintains a list of the top trending videos on the platform. According to Variety magazine, “To determine the year’s top-trending videos, YouTube uses a combination of factors including measuring users interactions (number of views, shares, comments and likes). Note that they’re not the most-viewed videos overall for the calendar year”. Top performers on the YouTube trending list are music videos (such as the famously virile “Gangam Style”), celebrity and/or reality TV performances, and the random dude-with-a-camera viral videos that YouTube is well-known for.

This dataset is a daily record of the top trending YouTube videos.

### Content
This dataset includes several months (and counting) of data on daily trending YouTube videos. Data is included for the US, GB, IN, DE, CA, and FR regions (USA, Great Britain, India, Germany, Canada, and France, respectively), with up to 200 listed trending videos per day.

Each region’s data is in a separate file. Data includes the video title, channel title, publish time, tags, views, likes and dislikes, description, and comment count.

The data also includes a category_id field, which varies between regions. To retrieve the categories for a specific video, find it in the associated JSON. One such file is included for each of the five regions in the dataset.

### Description
The dataset includes data gathered from videos on YouTube that are contained within the trending category each day. There are two kinds of data files, one includes comments and one includes video statistics. They are linked by the unique video_id field.

The headers in the video file are:

    video_id (Common id field to both comment and video csv files)
    title
    channel_title
    category_id (Can be looked up using the included JSON files, but varies per region so use the appropriate JSON file for the CSV file's country)
    tags (Separated by | character, [none] is displayed if there are no tags)
    views
    likes
    dislikes
    thumbnail_link
    date (Formatted like so: [day].[month])

The headers in the comments file are:

    video_id (Common id field to both comment and video csv files)
    comment_text
    likes
    replies
    
Extra info: The YouTube API is not effective at formatting comments by relevance, although it claims to do so. As a result, the most relevant comments do not align with the top comments at all, they aren't even sorted by likes or replies.

### Acknowledgements
This dataset was collected from Kaggle data. The information is same as that mentioned in the Kaggle Task window for the same.

### Reference Links

    1. https://www.kaggle.com/hoonkeng/deep-analysis-on-youtube-trending-videos-eda
    2. https://www.kaggle.com/ankkur13/sentiment-analysis-nlp-wordcloud-textblob 
    3. https://www.kaggle.com/somang1418/youtube-video-title-generator-by-lstm-eda#Finding-Outlier-Youtube-Video 
    4. https://www.kaggle.com/ammar111/youtube-trending-videos-analysis 

### Inspiration
Possible uses for this dataset could include:

    * Sentiment analysis in a variety of forms.
    * Categorising YouTube videos based on their comments and statistics.
    * Training ML algorithms like RNNs to generate their own YouTube comments.
    * Analysing what factors affect how popular a YouTube video will be.
    * Statistical analysis over time.
    
### Index 
The steps followed in the code to follow the outcome :-

    1. Importing Libraries
    2. Loading Dataset
    3. Understanding the dataset
    4. Data Cleaning
    5. Data Preparation
    6. Exploratory Data Analysis based on statistics
    7. Sentiment Analysis
    8. Insights Conclusion
    
    
### Aim 
The main focus in this project is based under following points :-

    # Analysing what factors affect how popular a YouTube video will be.
    # Trying sentiment analysis in a variety of forms.
