# IMDb-Movie-Sentiment-Analysis-with-Python
Sentiment Analysis is a common NLP task that Data Scientists need to perform. This is a straightforward guide to creating a barebones movie review classifier in Python. Future parts of this series will focus on improving the classifier.

Data Overview For this analysis we’ll be using a dataset of 50,000 movie reviews taken from IMDb.

The data is split evenly with 25k reviews intended for training and 25k for testing your classifier. Moreover, each set has 12.5k positive and 12.5k negative reviews.

IMDb lets users rate movies on a scale from 1 to 10. To label these reviews the curator of the data labeled anything with ≤ 4 stars as negative and anything with ≥ 7 stars as positive. Reviews with 5 or 6 stars were left out.
We’ve gone over several options for transforming text that can improve the accuracy of an NLP model. Which combination of these techniques will yield the best results will depend on the task, data representation, and algorithms you choose. It’s always a good idea to try out many different combinations to see what works.
I found that removing a small set of stop words along with an n-gram range from 1 to 3 and a linear support vector classifier gave me the best results.
We broke the 90% mark with the Final Accuracy: 0.90024.
