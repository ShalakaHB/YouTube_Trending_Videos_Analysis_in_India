# YouTube_Trending_Videos_Analysis_in_India
The YouTube Data Collection and Analysis project aims to gather data on YouTube videos using Google Cloud Console-generated YouTube APLs. 

![1684203163558](https://github.com/user-attachments/assets/2b2c5fdf-6435-4454-83c6-2114111fff61)

## Project Overview :
The YpuTube Data Collection and Analysis project aims to gather data on YouTube videos using Google Cloud Console-generated YouTube APLs. This project will focus on collecting data about trending videos in India and conducting an in-depth analysis to identify factors contributing to the popularity of these videos, such as video category, view count, like count, comment count, and video length. The analysis will provide valuable insights into user behaviour and content preferences, helping content creators and marketers make data-driven decisions. 

## Objectives :
- Data Collection: Use the YouTube Data API to extract data on trending videos, including video metadata, statistics, and user engagement metrics.
- Data Analysis: Analyze the collected data to uncover patterns and engagement ( views, likes, comments).
- Predictive Modeling: Develop predictive models to forecast video popularity based on historical data, helping creators optimise their content strategies.
- Visualisation: Create clear and insightful visualisations ( graphs, charts) to represent the trends and patterns discovered during the analysis.

## Dataset Description:
- video_id: Unique identifier for each video.
- title: Title of the video.
- description: Description provided by the video uploader.
- published_at: Date and time when the video was published.
- channel_id: Unique identifier for the YouTube channel.
- channel_titel: Name of the YouTube channel.
- category_id:  Numerical ID representing the category of the video.
- tags: A list of tags associated with the video.
- duration: Quality of the video (e.g., HD).
- caption: Boolean value indicating if captions are available.
- view_count: Number of views the video has received.
- like_count: Number of likes the video has received.
- dislike_count: Number of dislikes the video has received.
- favorite_count: Number of times the video has been favourited.
- comment_count: Number of comments the video has received.

## Scope :
The project will involve the following steps:
- API Integration: Set up the YpuTube Data API using Google Cloud Console and obtain access keys for data extraction.
- Data Collection: Collect data on trending videos, including:
    - Video Title 
    - Channel Name 
    - Category
    - Published Date
    - View Count
    - Like Count
    - Comment Count
    - Video Lenght 
    - Tags
    - Description
- Data Preprocessing: Clean and preprocess the data by handling missing or duplicate entries and formatting the dataset for analysis.
- Exploratory Data Analysis (EDA): Perform EDA to understand the key factors influencing video trends and user engagement. Analyze the following:
    - Most popular categories
    - Relationship between video length and view count 
    - Impact of publication time on popularity
    - Engagement metrics like likes and comments
- Machine Learning Models: Use regression or classification models to predict video popularity based on factors like category, tags, and user interaction data.
- Visualization: Create dashboards or interactive visualisations to present findings in a user-friendly manner.

## Tools And Technologies:
- Programming Language: Python
- API: YouTube Data APL v3 (Google Cloud Console)
- Data Processing: Pandas, NumPy
- Visualisation: Matplotlib, Seaborn, Plotly, Dash (for interactive dashboards)
- Machine Learning: Scikit-learn

##  Let’s have a look at the distribution of views, likes and comments of all the videos in the data:

![views,like,counts](https://github.com/user-attachments/assets/6b0caf6e-c357-4132-a5ac-d33aac154009)

The histograms show that the distributions of view counts, like counts, and comment counts are right-skewed, with most videos having lower counts and a few videos having very high counts.

## Here’s how we can analyze the number of trending videos by category:

![No of trending videos by catgory](https://github.com/user-attachments/assets/fd08c4d8-638e-4973-a1e8-04b60ed0614a)

The bar chart shows that the Entertainment, People & Blogs, Gaming and Music categories have the highest number of trending videos.

##  The content and the duration of videos:

![CONTENET and DURATION](https://github.com/user-attachments/assets/ccd24745-6e53-482b-8f63-bdc5a5f0896a)

The correlation between video length and view count, indicating longer videos tend to have higher view counts. Videos in the 60-120 minute range have the highest average view counts, likes, and comments. Engagement increases as video length increases.

## Let’s see if there’s an impact of the time a video is posted on its views:

![distribution of video by houre](https://github.com/user-attachments/assets/ecc69cec-28e4-4595-8aee-1b9d7247957f)

The distribution shows that most videos are published between 05:00 (5 AM)and 11:00 and 14:00 hours (11 AM – 2 PM), indicating this may be an optimal time for uploading videos. There is a very weak negative relationship between publish hour and view count, suggesting that the hour of publication has minimal impact on engagement metrics.

## Conclusion : 
So, here’s my conclusion on what makes a video trend on YouTube:
1. Encourage viewers to like and comment on videos to boost engagement metrics.
2. Aim to create shorter videos (under 5 minutes) for shorter engagement, especially for categories like Education and News & Politics.
3. Aim to create longer videos (60 to 120 minutes) for higher engagement, especially for categories like Science & Techonology and Entertainment.
4. Schedule video uploads around peak times (11 AM – 3 PM) to maximise initial views and engagement.
