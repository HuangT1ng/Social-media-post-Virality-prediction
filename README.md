# Social-media-post-Virality-prediction
##  Project overview:

This project aims to predict the virality of social media posts defined by the number of likes and comments. By analyzing various features such as post_type, caption, number of followers of an account etc, the model determines the potential of a post to go viral.

##  Dataset:
Dataset obtained from kaggle: https://www.kaggle.com/competitions/predict-viral-instagram-posts-advanced

Data contains: profilename, following, followers, post_type, captions etc

##  Current Approach：
Using a pretrained Roberta model fine-tuned for binary classification with whether (number of likes or comments > 10,000) as output and the rest of the attributes as inputs

### Model used: Roberta
A transformer model that has already been trained on large amounts of text data to understand language patterns.

## Result
The virality prediction model was evaluated using a test dataset, where 10% of the posts were labeled as viral and 90% as non-viral. 

The model achieved an overall accuracy of 92.35%. This means that the model correctly predicted whether a post is viral or non-viral in over 92% of the cases.

Non-Viral Posts (Class 0):

Precision: 0.96     
Recall: 0.95
F1-Score: 0.96

Viral Posts (Class 1):

Precision: 0.56
Recall: 0.61
F1-Score: 0.58

For viral posts, the model performs weaker compared to non-viral posts, with a precision of 0.56 and recall of 0.61. This is likely due to the imbalance in the dataset, where viral posts is only 10% of the total data. 
