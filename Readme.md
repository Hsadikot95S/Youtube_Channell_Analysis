# 1. Aims, objectives and background

## 1.1. Introduction

Founded in 2005, Youtube has grown to become the second largest search engine in the world (behind Google) that processes more than 3 billion searches per month. [[1]](https://www.mushroomnetworks.com/infographics/youtube---the-2nd-largest-search-engine-infographic/). It is, however, generally a myth how the Youtube algorithm works, what makes a video get views and be recommended over another. In fact, YouTube has one of the largest scale and most sophisticated industrial recommendation systems in existence [[2]](https://dl.acm.org/doi/10.1145/2959100.2959190). For new content creators, it is a challenge to understand why a video gets video and others do not. There are many "myths" around the success of a Youtube video [[3]](https://vidiq.com/blog/post/5-youtube-algorithm-myths-youtubers-need-to-know-about/), for example if the video has more likes or comments, or if the video is of a certain duration. It is also worth experimenting and looking for "trends" in the topics that Youtube channels are covering in a certain niche.

Having recently stepping into the content creation world with a new Youtube channel on data analytics and data science, I decided to gain some insights on this topic which might be useful for other new content creators. The scope of this small project is limited to data science channels and I will not consider other niches (that might have a different characteristics and audience base). Therefore, in this project will explore the statistics of around 10 most successful data science Youtube channel.

## 1.2. Aims and objectives

Within this project, I would like to explore the following:

- Getting to know Youtube API and how to obtain video data.
- Analyzing video data and verify different common "myths" about what makes a video do well on Youtube, for example:
    - Does the number of likes and comments matter for a video to get more views?
    - Does the video duration matter for views and interaction (likes/ comments)?
    - Does title length matter for views?
    - How many tags do good performing videos have? What are the common tags among these videos?
    - Across all the creators I take into consideration, how often do they upload new videos? On which days in the week?
- Explore the trending topics using NLP techniques
    - Which popular topics are being covered in the videos (e.g. using wordcloud for video titles)?
    - Which questions are being asked in the comment sections in the videos

## 1.3. Steps of the project
1. Obtain video meta data via Youtube API for the top 10-15 channels in the data science niche (this includes several small steps: create a developer key, request data and transform the responses into a usable data format)
2. Prepocess data and engineer additional features for analysis
3. Exploratory data analysis
4. Conclusions

## 1.4 Connecting the df to a database

1. To connect the df to a database I have first created a project in google cloud
2. After that i have created a dataset in the bigquery console named Youtube Analytics
3. After this I have created a table with the name of Youtube Comments

## 1.5 Significance of all the files used in the project:

1. Download_Data: Used to Download the video statistics for each channel identified by channel and playlist id. After we download the video statistics and convert the same to a df we convert the df to a csv file to be used for further analysis
2. Statistical_Analysis: Used to perform statistical analysis on the obtained df in step 1
3. EDA_Single_Channel: Performs EDA on a single channel
4. EDA: Performs EDA on all the 5 channels combined
5. Database: Connects to a big query database and uploads a df over there


