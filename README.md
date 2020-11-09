# NLP-Twitter-Disaster-Tweets


Competition Description

Twitter has become an important communication channel in times of emergency. The ubiquitousness of smartphones enables people to announce an emergency they’re observing in real-time. Because of this, more agencies are interested in programatically monitoring Twitter (i.e. disaster relief organizations and news agencies).

But, it’s not always clear whether a person’s words are actually announcing a disaster.

When we first started learning about NLP, we chose to write this kernel. It is essentially the stuff we have learned documented in Kaggle Notebook format.

It can be helpful for you if you are looking for data analysis on competition data, feature engineering ideas for NLP, cleaning and text processing ideas, and Logistic Regression.

Datasets:

Datasets Used In This Notebook Are As Follows

Real or Not? NLP with Disaster Tweets
Disasters on social media

Import Libraries

![image-1](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-1.JPG)

Visualization with the class imbalance thing

![image-2](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-2.JPG)


2. Keywords

![image-3](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-3.JPG)

![image-4](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-4.JPG)

![image-5](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-5.JPG)

3. Locations

![image-6](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-6.JPG)

![image-7](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-7.JPG)

Data Preprocessing Part

![image-8](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-8.JPG)


Cleaning the Data
5. Clean up Text Column

Here we clean up the text column by:

    Making a 'clean' text column, removing links and unnecessary white spaces
    Creating separate columns containing lists of hashtags, mentions, and links
    
![image-9](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-9.JPG)    

6. Create statistics from texts

![image-10](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-10.JPG) 


7. Most frequent words and bigrams

What are the most common unigrams (single word) and bigrams (two-word sequence)?

![image-11](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-11.JPG)

![image-12](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-12.JPG)

![image-13](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-13.JPG)


Feature Engineering
8. Encoding and Vectorizers

As part of feature generation, we will:

    Apply target encoding to keyword and location (cleaned)
    Count Vectorize cleaned text, links, hashtags and mentions columns

![image-14](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-14.JPG)

![image-15](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-15.JPG)

![image-16](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-16.JPG)

TF-IDF Count

![image-17](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-17.JPG)


Regression Technique
9. Logistic Regression

We try the simplest model with logistic regression, based on all features we created above. Before we fit a model, we first transform the features into the same scale with minimum 0 and maximum 1. We do this in the form of pipeline.

![image-18](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-18.JPG)

F1 SCORE

![image-19](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-19.JPG)

Confusion matrix

![image-20](https://github.com/hemangikinger/NLP-Twitter-Disaster-Tweets/blob/master/image-20.JPG)


