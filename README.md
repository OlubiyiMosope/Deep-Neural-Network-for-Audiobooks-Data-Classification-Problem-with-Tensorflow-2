# Deep-Neural-Network-for-Audiobooks-Data-Classification-Problem-with-Tensorflow-2

This project employs a deep neural network model to determine whether or not an audio book app user will make another purchase on the platform based on purchase, and usage data collected over a two year period..


### Problem Description
This is a project that employs a deep neural network model to determine whether or not an audio book app user will make another purchase on the platform based on purchase, and usage data collected over a two year period.

The data is from an Audiobook App. Logically, it relates to the audio versions of books ONLY. Each customer in the database has made a purchase at least once, that's why they are in the database.  
The objective is to create a machine learning algorithm based on our available data that can predict if a customer will buy again from the Audiobook company.

The main idea is that if a customer has a low probability of coming back, there is no reason to spend any money on advertising to him/her. If we can focus our efforts SOLELY on customers that are likely to convert again, we can make great savings. Moreover, this model can identify the most important metrics for a customer to come back again. Identifying new customers creates value and growth opportunities.

###### Dataset Summary
You have a `.csv` summarizing the data. There are several variables: 
- Customer ID,
- Book length overall (sum of the minute length of all purchases), 
- Book length avg (average length in minutes of all purchases),
- Price paid_overall (sum of all purchases), 
- Price Paid avg (average of all purchases), 
- Review (a Boolean variable whether the customer left a review), 
- Review out of 10 (if the customer left a review, his/her review out of 10), 
- Total minutes listened, 
- Completion, 
- Support requests (number of support requests; everything from forgotten password to assistance for using the App), and 
- Last visited minus purchase date (in days).

These are the input features of the dataset.

The target is a Boolean variable (0 or 1). The data for the inputs is collected over a period of 2 years. Data of whether a customer churns or not is taken at the end of following six (6) months following the initial 2 year period.
So, in fact, we are predicting if: based on the last 2 years of activity and engagement, a customer will convert in the next 6 months. If they don't convert after 6 months, chances are they've gone to a competitor or didn't like the Audiobook way of digesting information.

###### Objective
The task is simple: create a machine learning algorithm, which is able to predict if a customer will buy again.

This is a binary classification problem with two classes: won't buy and will buy, represented by 0s and 1s.
- 1: The customer converted
- 0: The customer did not convert.
