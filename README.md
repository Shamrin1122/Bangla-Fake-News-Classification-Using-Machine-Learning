Problem Statement

Nowadays, everything is getting digitalized. So, with the blessings of modern technology, people can read news of the whole world through different kinds of online news portals. A large number of people in our country now read online news portals in Bengali. Among these news portals, there also have some fake news and real news. But, in maximum time mass people can’t discriminate between this two. That’s why it is necessary to classify fake news and real news. In this project, we use different kinds of machine learning models such as Random Forest, Logistic Regression, KNN, and Decision Tree for the dataset named “BanFakeNews” to classify whether the news is real or fake. Among these models, Logistic Regression comparatively performs better gaining 92%.



Dataset
The provided dataset contains around 8.5k news data on the different news portals. Between these, around 7k are authentic, and around 1k are fake news. The fake news is labeled with 0 and the real news is labeled with 1.


![Screenshot (36)](https://user-images.githubusercontent.com/114852884/214569868-ed335830-6a25-406b-84d8-5092743414d0.png)

 Fig. 1. Histogram of frequency and content length
                                              
                                              
                                              
                        
Approach


 The dataset contains raw data and we have cleaned this dataset by removing stop-words, special characters, and punctuations in the pre-processing stage. For separating every word, we have used here tokenization. Then we extracted the features from the news data using TF-IDF. The following diagram is for workflow:



![Screenshot (38)](https://user-images.githubusercontent.com/114852884/214570316-7ff7d8bc-240c-414d-b8ef-96c6eccbca33.png)


We have classified the news according to the following steps:

Step 1:  Load the dataset.

Step 2:  Remove stop words, punctuations, and special characters.

Step 3:  Use TF-IDF for feature extraction.

Step 4: Then split the dataset into 70% and 30% where 70% is for training and 30% is for testing part.  

Step 5:  Use Machine learning models (Random Forest, Logistic Regression, KNN, Decision Tree).
   
Step 6:   Calculate Recall, Precision, F1 Score, and Accuracy for every model. From these Metrics, we have got the best model for which we have got the best accuracy.

