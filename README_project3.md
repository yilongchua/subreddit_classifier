Project 3: Web APIs & Classification

### Description

For project 3, your goal is two-fold:
1. Using Reddit's API, you'll collect posts from two subreddits of your choosing.
2. You'll then use NLP to train a classifier on which subreddit a given post came from. This is a binary classification problem.

## Reddit Background and topics choosen for project
Reddit is a collection of online discussion boards known as "subreddits", which cover a variety of topics. The goal of this project is to classify which subreddit a given post came from. There are [over 1.5 million subreddits](http://redditmetrics.com/history) on reddit, 

we will be classifying posts from two subreddits, [/r/Marriage] and [/r/Divorce], to make the project manageable. The choice of these two subreddits is motivated by their proximately in terms of topic closeness and text-driven post.

We will be creating and comparing two models: a logistic regression and a multinomial naive Bayes classifier. Our results may be useful for any reddit user who is unsure which subreddit is the most appropriate to submit his new post, so that he can attract the most comments.

### Background           : 
With falling birthrates in singapore, there is a need to understand the issues faced by couples entering or exiting marriage. In order to start off this study, 100,000 couples choose to give their consent to their social media accounts. However it is unclear about their current 'marriage' status.

### Problem statement    : 
There is a need to segregate these couples into their martial status category. Asking this question might be sensitive, especially towards couples 'recencently divorced'. Hence come out with a classifier based on the 2 topics to classify these 100,000 couples into their martial status. 

Topics choosen: 
                1. Marriage
                2. Divorice

Classify any written post on the 2 topics choosen into the correct categories. 

### My position          :
My position is as a data science consultant to the agency conducting this study.

### My Audience Position :
My audience position is the agency carrying out this martial study.


### Contents:
- [1. Data Collection]
- [2. Data Cleaning and EDA]
- [3. Modeling]
- [4. Conclusion and Recommendations]

## Data Dictionary
textfeature.csv
Feature|Type|Description
---|---|---
**textfeature**|_object_|Body text of a post.
**subreddit**|_int_|"1" represent Topic 1, Marriage. "0" represent topic 2, Divorce.


## Conclusion and Recommendations

- Our TifdfVectoriser with Logistic Regression classifier performed best out of all 4 models. 

- The difference in the train and test score is slightly wider than expected. This is probably due to the high amount of features choosen (3000 features per model selected). 

- The accuracy score of 84% is slightly higher than expected, as seen in the dataframe above. This is within expectations because the topics of our two chosen subreddits differ slightly.

- Scope for future improvements:
    - Optimize stop words and explore strategies for stemming and lemmatization
    - Try ensemble models, such as random forest classifier
    - Ability for model to classify more than two subreddits

