# recommendations-with-IBM
In this project which is a part of Udacity nanodegree program,  four different recommendation systems to on real data from the IBM Watson Studio platform is studied:
- Rank Based Recommendation.
- User-User Based Collaborative Filtering.
- Content Based Recommendations.
- Matrix Factorization. 

### Table of Contents

1. [Requirements](#libraries)
2. [Files](#files)
3. [Workflow](#analysis)


## Packges  <a name="libraries"></a>
The project was implemented using Anaconda distribution of Python 3.0. Moreover I have used the following python libraries:

1. Pickle
2. Matplotlib
3. NLTK
4. NumPy
5. Pandas


## File Descriptions <a name="files"></a>

The Jupyter notebook showcases the analysis done in order to explore the dataset, the data preparation and wrangling as well as the building of recommendation engine. The notebook contains markdown cells to help with documentation of the steps.

For reference an HTML version of the notebook is also available.

Lastly, the data folder contains the dataset from IBM Watson Studio platform.
It contains 3 files:

- articles_community.csv:  articles descriptive information 
- user-item-interactions.csv: users interactions with articles 

## Analysis Workflow  <a name="analysis"></a>

#### Exploratory Data Analysis
Before making recommendations of any kind, I explored the data to identify any missing values and data distribution. I cleaned and prepared the data for the analysis.

#### Rank Based Recommendations
To get started in building recommendations, I first identified the most popular articles simply based on users interaction. Since there are no ratings for any of those articles, it made sense to assume that articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

#### User-User Based Collaborative Filtering
In order to build better recommendations for the users of IBM's platform, I took a look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users.

#### Content Based Recommendations
Given the amount of content available for each article, there are a number of different ways in which someone might choose to implement a content based recommendations system. I utilized NLP to develop a content based recommendation system. This system goes through each article title and finds the most common words(related to a content) throughout all the available articles and recommends articles based on the sum of matched words in the title of an article and popularity.

#### Matrix Factorization
Matrix decomposition is used to predict new articles an individual might interact with.
