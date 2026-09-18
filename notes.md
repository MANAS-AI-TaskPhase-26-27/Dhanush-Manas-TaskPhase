Notes for ML-

* Machine learning is a powerful technology we use in our day to day lives but never even know about it
* It allows humans to solve problems in a new way, answer complex questions and also create new content.
* Machine learning is basically training a software called a model and then using to make predictions or classifications or generate content from data.
* Training means basically feeding the model a lot of data and based on the type of model the ML performs different actions on it. The larger the amount of data more the accuracy
* One of the best ways to use ML is in prediction, prediction of weather or prediction of stock market ( quant )
* Mainly there are 4 types of ML models :

  1. Supervised Learning
  2. Unsupervised Learning
  3. Reinforcment Learning
  4. Generative AI
  * Supervised learning models are used in scenarios where predictions or classifications are required. The model knows the question and the answer and will predict the answer for a future question basically. There are three types of models in Supervised learning:

    * Regression - Uses past data to predict future numerical values, for example stock market prices or price of real estate or price of vegetables
    * Binary Classifcation - Based on already know datas and category of each data it will classify any new data given to it into each category, and binary for only two available values / categories
    * Multi classification - same as binary except for two there are a multitude of categories available



* Unsupervised learning models are used when you have unlabelled set of data and you want to classify it into different groups, the model basically clusters(k-nearest neighbours, hierarchal) the data into each cluster. It doesn't know what each cluster signifies but it will be able to make the clusters themselves. We must name the cluster ourselves for our understanding. Its useful for finding patterns when we dont have any pattern or connection between data for example relation of climate and all the years in history. Another type of unsupervised learning is dimensionality reduction.
* Reinforcement learning - basically what us humans are taught in school, based on how well a model performs a reward is given. It generates a policy that lets it gets the most rewards for what actions it performs.
* Generative Ai- it uses data of similar sort to generate newer data, its like observing other sports person to learn the sport yourself. there are multiple classifications based on what conversion to generation. Like text-to-text, text-to-vid etc.



A supervised learning model is based on the following core concepts: -

* Data - Data has a feature and a label. Data must be large and highly diverse for the model to be as accurate as possible. Feature is basically the values of data and label is the type of value.
* Model - Model is basically a mathematical collection of numbers and relations that is used to predict / classify data
* Training - any supervised learning model uses predicted value vs actual value to train itself and find the most accurate mathematical relation to predict values. It uses a difference called loss between predicted and actual values. Once the predicted values start matching the actual values the model is ready for evaluation
* Evaluation - Evaluation is basically testing the model with new data. if the values provided by the data matches the actual values then the model is ready for future use
* inference - basically actually using the model in  the real world, using unlabelled data obviously.



Machine learning is not the same as AI, it is a subset of AI and deep learning is a subset of Machine learning.





Now next about data.

&#x20;Data cleaning is an essential step for a model to learn effectively during the training phase. It involves identifying errors, handling and correcting them, or fixing inconsistencies in the data. Its basically just making the data as accurate and useful as possible.

Firstly we learn how to handle missing values. For missing values you either keep them as NaN if they dont exist but if they exist and have not been recorded you guess them, and this is called imputation.

to handle missing values we can either drop the rows/columns corresponding to them or fill in the missing values.

We then learn about scaling and normalization. Scaling is changing the range of your data and normalization is the changing the shape of the distribution of the data. we use minmax\_scaling() for scaling and

stats.boxcox() for normalization

we also learnt about parsing dates, here we turn the dates that are originally recorded as strings to proper date datatype. we use pd.to\_datatime to parse dates



next we learn character encodings

Usually all data is stored in utf-8 encoding but sometimes it may be in different one, so we use charaset\_normalizer to guess the encoding so that when reading the data we will not have any errors.

we also learnt how to save a csv file under a certain encoding



new we learnt how to fix typos in data. we use the module fuzzy wuzzy to match strings of the same type and then replace all those that match the closest with another string.



I then next learn what is overfitting and underfitting. In underfitting a model is too simple and doesn't grasp any patterns in a data and an overfitting model will just memorize the data instead of finding patterns in it, so the model performs well in the training phase but not in the evaluation and inference phase. Both are unnecessary in machine learning.



Lastly i learnt about evaluation metrics, there are different metrics based on the model. For a supervised learning model there are two types, one is classification and other is regression

in classification the metrics are - (outcomes are true positive, true negative, false positive, false negative)

* accuracy - to measure how much a model matches the real and correct answer
* precision - to measure how each time it predicts how close is each prediction to the actual answer
* recall - out of all the positives, how many did the model actually find, did anything slip by
* f1 score - harmonic mean of precision and recall. Higher the score the more true positives the model gives without false positives or negatives.

then there are metrics in reggression-

* absolute error, root mean square error, mean squared error,etc.



This is all i have learnt about ML up until now, i will need more practice but i think i know most of it on a high level.





