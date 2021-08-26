    
# Recommendations with IBM

### Table of Contents   
1. [Description](#description)
2. [Installation](#installation)
3. [File Descriptions](#files)
4. [Licensing, Authors, and Acknowledgements](#licensing)

## Description<a name="description"></a>

For this project, I analyzed the interactions that users have with articles on the [IBM Watson Studio platform](https://dataplatform.cloud.ibm.com/login), and make recommendations to them about new articles I think they will like. Below is an example of what the dashboard could look like displaying articles on the IBM Watson Platform.

![Lanes Image](./doc/IBM Watson Studio platform.png)

The project is divided into the following tasks

### I. Exploratory Data Analysis

Explore the data for the project. 

### II. Rank Based Recommendations

To get started in building recommendations, I found the most popular articles simply based on the most interactions. Since there are no ratings for any of the articles, it is easy to assume the articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

### III. User-User Based Collaborative Filtering

In order to build better recommendations for the users of IBM's platform, we could look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users.

### IV. Content Based Recommendations (EXTRA - Future implementation)

Given the amount of content available for each article, there are a number of different ways in which someone might choose to implement a content based recommendations system. Using your NLP skills to develop a content based recommendation system. 

### V. Matrix Factorization

Finally, I used a machine learning approach to building recommendations. Using the user-item interactions, I built out a matrix decomposition. Using Singular Value Decomposition from numpy on the user-item matrix. 

Unfortunately, test accuracy goes down with increasing latent features, so accuracy is not a good metric, predicted interactions are imbalanced. This can be a case of faillure to generalize the model (overfitting).


## Installation <a name="installation"></a>

Reguired installations:

* Jupyter Notebooks (Anaconda Distribution)
* Python 3.8.5

Required packages:

* Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
* Model Loading and Saving Library: Pickle
* Data Visualization: Plotly


## File Descriptions <a name="files"></a>

1. data:
    * Provided by IBM in collaboration with Udacity.
    * `data\articles_community.csv` :
    * `data\user-item-interactions` :    
    
2. model:
    * `Recommendations_with_IBM.ipynb`: My answer for recommendations, It describe how to recommend articles to users
    * `Recommendations_with_IBM.html`: As the same of above notebook but format is html.


## Licensing, Authors, Acknowledgements<a name="licensing"></a>

This project was completed as part of the [Udacity Data Scientist Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025).

