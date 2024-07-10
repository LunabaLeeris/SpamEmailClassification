# What is this about ?

This is a case study on the effectiveness of Naive Bayes + Laplace smoothing in learning to predict whether an email is a spam or ham (legitimate). 

Specifically this experiment aims to differentiate the following versions of Naive Bayes:

1. Multi-variate Bernoulli Event Model (MVBEM)
2. Multi-nomial Event Model (MNEM)

# Data 

NOTE: Control data corresponds to the data in which the model is not trained on

Training data gathered from: https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset/data
Control data gathered from: https://www.kaggle.com/datasets/prishasawhney/email-classification-ham-spam

Training data has length 5169, 87% of which are ham emails
Control data has length 179, 56% of which is ham 

# Summary of Results

1. Using the configs in the main.ipynb file the overall session took 10 mins to complete. 
2. The overall session occupied 4gb RAM 
3. MNEM have a slight advantage in terms of accuracy compared to MVBEM
4. Both models had 99% accuracy using the Training Dataset
5. Both models have 60-65% accuracy using the Control Dataset 
6. Both models have a hard time classifying Spam Emails. This may be due to the fact that ham emails are low compared to ham emails. 
7. MNEM is better at classifying Spam Emails 
8. MVBEM is better at classifying Ham Emails
9. MNEM is generally better than MVBEM

# Future Improvements and Recommendations

1. Some of the functions can be reduced to singular functions. 
2. Future studies may take into account the following factors
   -Mispellings
   -Capitalizations
   -Special Characters
   -Links 
3. Both method uses binary classification. Maybe generalize the methods to multi-class ? 
4. Both methods does not take into account the position of words in the text. Try a new model which delves into this and compare whether   there is a significant difference in accuracy. 
