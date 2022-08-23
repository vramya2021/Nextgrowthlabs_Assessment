# Nextgrowthlabs_Assessment

Question 1: Write about any difficult problem that you solved. (According to us difficult - is something which 90% of people would have only 10% probability in getting a similarly good solution). 

During my masters in Data Science, I have done Emotion Recognition project where emotions are the key to understanding human interactions especially those conveyed with facial expressions. Handling dataset with thousands of images from the internet causing memory of high usage was the difficult situation. But I have used Google colab because it supports high GPU and performance was better during my Capstone Professional project.


Question 2: Explain back propagation and tell us how you handle a dataset if 4 out of 30 parameters have null values more than 40 percentage

Backpropagation is an algorithm used in artificial intelligence (AI) to fine-tune mathematical weight functions and improve the accuracy of an artificial neural network's outputs. The following are the some ways to handle 

1.Predicting The Missing Values
Using the features which do not have missing values, we can predict the nulls with the help of a machine learning algorithm. This method may result in better accuracy, unless a missing value is expected to have a very high variance. 

2.Replacing with Mean, Mean and Mode
This strategy can be applied on a feature which has numeric data like the age of a person or the ticket fare. We can calculate the mean, median or mode of the feature and replace it with the missing values. This is an approximation which can add variance to the data set. But the loss of the data can be negated by this method which yields better results compared to removal of rows and columns. Replacing with the above three approximations are a statistical approach of handling the missing values. This method is also called as leaking the data while training. Another way is to approximate it with the deviation of neighbouring values. This works better if the data is linear.  

3.Assigning An Unique Category
A categorical feature will have a definite number of possibilities, such as gender, for example. Since they have a definite number of classes, we can assign another class for the missing values. Here, the features Cabin and Embarked have missing values which can be replaced with a new category, say, U for ‘unknown’. This strategy will add more information into the dataset which will result in the change of variance. Since they are categorical, we need to find one hot encoding to convert it to a numeric form for the algorithm to understand it

4.Using Algorithms Which Support Missing Values
KNN is a machine learning algorithm which works on the principle of distance measure. This algorithm can be used when there are nulls present in the dataset. While the algorithm is applied, KNN considers the missing values by taking the majority of the K nearest values.
