# NaiveBayes

1. Naïve Bayes algorithm is a supervised learning algorithm, which is based on Bayes theorem and used for solving classification problems.
2. It is mainly used in text classification that includes a high-dimensional training dataset.
3. Naïve Bayes Classifier is one of the simple and most effective Classification algorithms which helps in building the fast machine learning models that can make quick predictions.
4. It is a probabilistic classifier, which means it predicts on the basis of the probability of an object.


Bayes' theorem is also known as Bayes' Rule or Bayes' law, which is used to determine the probability of a hypothesis with prior knowledge. It depends on the conditional probability.

TYPES OF NAIVE BAYES:

1. Gaussian:    a. Assumes that features follow Normal Distribution.
                b. Predictors take ontinuous values insted of discrete.
                c. Model assumes values are sampled from Gaussian Distribution.
from sklearn.naive_bayes import GaussianNB  
classifier = GaussianNB()  
classifier.fit(x_train, y_train)

2. Multinomial: a. Data is multinomially distributed.
                b. Used for Document Classifications.
                c. Uses Frequency of Words for prediction
        
3. Bernoulli:   a. Similar to MultiNomial but Predictor values are independent boolean variables (word present in document or not) 1 or 0
                b. Also used for document classification tasks - One application would be text classification with ‘bag of words’ model
                
                

Main Application:
Text classification/ Spam Filtering/ Sentiment Analysis

