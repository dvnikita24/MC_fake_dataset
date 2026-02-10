# MC_fake_dataset
Repository to store MC_Fake dataset 


MC-Fake dataset
Introduction
The popularity of social media in recent years has promoted the spread of fake news. Detecting fake news on social media is challenging, as pieces of fake news pieces are intentionally written to mislead consumers, which means that it is often not possible to spot fake news from news content itself. For this reason, social context based detection methods, which attempt to model the spreading patterns of fake news by utilising the collective wisdom from users on social media, have been attracting increasing attention. In response to this, the MC-Fake dataset has been created to facilitate the detection of fake news using such methods.

Dataset description
The MC-Fake fake news dataset contains 28334 news events on multiple topics (Politics, Entertainment, Health, Covid-19, Syria War) and corresponding social context (tweets, retweets, replies, users, retweet_relations, replying relations, user-follows-user relations) collected from Twitter.

Dataset format
The majority of information about the news articles and their corresponding social context is provided in the form of a csv file. The user-follows-user relations are provided in a separate social network file. The format of both types of files is described below.

csv file
The news dataset and corresponding social context (apart from user-follows-user relations, which are in the separate social network file, see below) are provided in the form of csv 
files, consisting of 16 columns:
**news_id**: the id of the news event
**title**: title of the news
**url**: source url of the news
**publish_date**: publish date
**source**: news source
**text**: text content of the news
**labels**: veracity label of the news
**n_tweets**: tweet counts
**n_retweets**: retweet counts
**n_replies**: reply counts
**n_users**: user counts
**tweet_ids**: IDs of the relevant tweets, separated by commas
**retweet_ids**: IDs of the relevant retweets, separated by commas
**reply_ids**: IDs of the relevant replies, separated by commas
**user_ids**: IDs of the relevant users, separated by commas
**retweet_relations**: retweet relations indicated by a list of tokens {tweet_ID_A}-{tweet_ID_B}-{user_ID of tweet A}-{user_ID of tweet B} denoting A retweets
**reply_relations**: reply relations indicated by a list of tokens {tweet_ID_A}-{tweet_ID_B}-{user_ID of tweet A}-{user_ID of tweet B} denoting A replies B
**data_name**: news category


The dataset was constructed at the National Centre for Text Mining (NaCTeM), School of Computer Science, University of Manchester, UK. It is licensed under a Creative Commons Attribution 4.0 International License. Please attribute NaCTeM when using the dataset, and please cite the following article:

Min, E., Rong, Y, Xu, T., Bian, Y., Zhao, P., Huang, J. and Ananiadou, S. (2022). Divide-and-Conquer: Post-User Interaction Network for Fake News Detection on Social Media. In: Proceedings of The Web Conference 2022, pp. 1148-1158.
