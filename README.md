Social_Media_Sentiment_Analysis
About Dataset
This dataset is a Kaggle Dataset named 'Social Media Sentiments Analysis Dataset'
It captures a vibrant tapestry of emotions, trends, and interactions across various social media platforms.
This dataset provides a snapshot of user-generated content, encompassing text, timestamps, hashtags, countries, likes, and retweets. Each entry unveils unique stories—moments of surprise, excitement, admiration, thrill, contentment, and more—shared by individuals worldwide.

Description :
   
This project aims to understand sentiment changes from 2010 to 2023 on popular social media platforms based on certain attributes and how they impact each other.
This project explores the standard procedure of data analysis, including data preprocessing, feature engineering, EDA and NLP tasks
This project introduces the standard procedure of natural language processing(text clearning, word embedding, etc.), and used multiclass classification models for sentiment analysis.
This project leverages some popular data-analyic tools, including pandas, matplotlib, seaborn and a decent usage of natural language processing tool-nltk.
This project can serve as a beginner-friendly tutorial on data analysis and data visualization.

PROCESS FOLLOWED :

1️. Data Loading & Initial Inspection
Dataset: sentimentdataset.csv

Initial Inspection:

Removed unnecessary columns (e.g., unnamed index columns).

Identified key columns for analysis: Text, Timestamp, Platform, Country, and Sentiment.

2️. Data Cleaning
Duplicate Removal: Ensured that duplicate rows do not bias the analysis.

Handling Missing/Incorrect Values: Null values were not present, so removed duplicated  values and

Timestamp Conversion: Converted Timestamp to a proper datetime format for time-based analysis.

3️. Feature Engineering
Temporal Features: Extracted Day_of_week and Month from the Timestamp column.

-- It Helps identify patterns in sentiment across days of the week and months.

Text Processing: Created a new column Clean_Text by processing the raw Text for consistency and standardization.

4️. Text Preprocessing (NLP Basics)
Standardized the text by:

Converting to lowercase.

Removing URLs, mentions (@user), hashtags, punctuation, and numbers.

This step ensures that the text is ready for further NLP tasks, including sentiment analysis.

5️. Exploratory Data Analysis (EDA)
Sentiment Distribution: Visualized the distribution of sentiment labels (positive, negative, neutral).

Monthly Sentiment Trend: Analyzed how sentiment types change over time, tracking sentiment shifts based on the cleaned Timestamp.

6️. Model-Based Sentiment Scoring 
VADER Sentiment Analysis: Integrated VADER, a pre-trained lexicon-based sentiment analysis model.

Calculated a compound sentiment score for each post.

Created a new column Predicted_Sentiment, which classifies posts as positive, negative, or neutral based on the sentiment score.

7️. Time-Based Sentiment Trends
Resampling: Resampled the data weekly to track sentiment trends.

Sentiment Trends Visualization: Plotted the average sentiment trends over time, offering insights into public sentiment shifts.

8️. Platform-Wise and Word-Level Insights
Platform-Based Sentiment Breakdown: Aiming to compare sentiment across different platforms (e.g., Twitter, Facebook).

Word Clouds: Planned creation of word clouds to explore frequent words in positive, negative, and neutral posts.