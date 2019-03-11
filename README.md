# Recommendations_with_IBM
This project is about building article recommender systems to users in IBM
Waston Studio based upon current user-article interactions in this platform.

Multilple recommendation methods have been implemented in this project.

This project is from Udacity Data Science Nano-Degree and data comes from [IBM
Waston Studio](https://dataplatform.cloud.ibm.com)


## Project Outline

* Exploratory Data Analysis
* Rank Based Recommendations
* User-User Based Collaborative Filtering
* Content-Based Recommendations (NLP applied)
* Matrix Factorization Recommendation (SVD model applied)


### **1**. **Exploratory Data Analysis**
Before building recommender systems, basic data exploratory was implemented.
For example: total user number, total article number, most viewed articles,
viewed times distributions, etc. Also, certain data cleaning and feature
engineering will be applied in this part.

### **2**. **Rank Based Recommendations**
By getting started, the recommendation system was simply upon the interaction
frequency. The most interacted articles would be treated as most popular ones
to be recommended. This method would be a good choice for new users who have no
article viewing history.

### **3**. **User-User Based Collaborative Filtering**
This method utilized the user-article interactions to make recommendations.
Users would be recommended articles viewed by users who have similar article
interactions. This way is more personalized comparing with rank based method.

### **4**. **Content-Based Recommendations**
The content-based method was upon the article similarities to do
recommendation. Natural Language Processing and tf-idf were applied on article
titles for calculating the similarities. Current users will be recommended
similar articles with what they have viewed in history. The most popular articles
and their most similar articles will be recommended to new users. This method is
good for new articles have no viewing before.

### **5**. **Matrix Factorization Recommendation**
Machine Learning approach (SVD -- Singular Value Decomposition) was applied in
this part. By utilizing user-article interactions, matrix decomposition was
built. Also, training and testing dataset were splitting to find the best latent
feature numbers and model evaluations.


## Required packages
nltk==3.4 <br />

In udacity workspace python:
`import nltk`
`nltk.download('stopwords')`
