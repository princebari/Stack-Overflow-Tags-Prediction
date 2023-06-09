# Stack-Overflow-Tags-Prediction
This repository contains the code and resources for an case study on Stack Overflow Tags Prediction using machine learning.

![image](https://github.com/princebari/Stack-Overflow-Tags-Prediction/assets/115543070/940f4d50-aa64-4096-a9a0-9c869e0e79ac)
<h2> Description </h2>
Stack Overflow is the largest, most trusted online community for developers to learn, share their programming knowledge, and build their careers.

Stack Overflow is something which every programmer use one way or another. Each month, over 50 million developers come to Stack Overflow to learn, share their knowledge, and build their careers. It features questions and answers on a wide range of topics in computer programming. The website serves as a platform for users to ask and answer questions, and, through membership and active participation, to vote questions and answers up or down and edit questions and answers in a fashion similar to a wiki or Digg. As of April 2014 Stack Overflow has over 4,000,000 registered users, and it exceeded 10,000,000 questions in late August 2015. Based on the type of tags assigned to questions, the top eight most discussed topics on the site are: Java, JavaScript, C#, PHP, Android, jQuery, Python and HTML.


<h2>Problem Statement</h2>

Suggest the tags based on the content that was there in the question posted on Stackoverflow.

<h2>Real World Objective and Business Constraints</h2>

*    Predict as many tags as possible with high precision and recall.
*   Incorrect tags could impact customer experience on StackOverflow.
*    No strict latency constraints.

<h2>Dataset URL</h2>

Refer : https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/

<h2> Type of Machine Learning Problem </h2>

It is a multi-label classification problem
Multi-label Classification: Multilabel classification assigns to each sample a set of target labels. This can be thought as predicting properties of a data-point that are not mutually exclusive, such as topics that are relevant for a document. A question on Stackoverflow might be about any of C, Pointers, FileIO and/or memory-management at the same time or none of these.

<h2>Perfomance Metric </h2>

Micro-Averaged F1-Score (Mean F Score) : The F1 score can be interpreted as a weighted average of the precision and recall, where an F1 score reaches its best value at 1 and worst score at 0. The relative contribution of precision and recall to the F1 score are equal. The formula for the F1 score is:

F1 = 2 * (precision * recall) / (precision + recall)

In the multi-class and multi-label case, this is the weighted average of the F1 score of each class.

'Micro f1 score':
Calculate metrics globally by counting the total true positives, false negatives and false positives. This is a better metric when we have class imbalance.

'Macro f1 score':
Calculate metrics for each label, and find their unweighted mean. This does not take label imbalance into account.

https://www.kaggle.com/wiki/MeanFScore
http://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html

Hamming loss : The Hamming loss is the fraction of labels that are incorrectly predicted.
https://www.kaggle.com/wiki/HammingLoss
