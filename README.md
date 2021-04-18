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



Points to Note:
1. If categorical variable has a category (in test data set), which was not observed in training data set, then model will assign a 0 (zero) probability and will be unable to make a prediction. This is often known as “Zero Frequency”.
    - To solve this: we can use the smoothing technique. One of the simplest smoothing techniques is called Laplace estimation.
2. Another limitation of Naive Bayes is the assumption of independent predictors. In real life, it is almost impossible that we get a set of predictors which are completely independent.


Tips:
1. If continuous features do not have normal distribution, we should use transformation or different methods to convert it in normal distribution.
2. If test data set has zero frequency issue, apply smoothing techniques “Laplace Correction” to predict the class of test data set.
3. Remove correlated features, as the highly correlated features are voted twice in the model and it can lead to over inflating importance.
4. Naive Bayes classifiers has limited options for parameter tuning like alpha=1 for smoothing, fit_prior=[True|False] to learn class prior probabilities or not.
5. You might think to apply some classifier combination technique like ensembling, bagging and boosting but these methods would not help. Actually, “ensembling, boosting, bagging” won’t help since their purpose is to reduce variance. Naive Bayes has no variance to minimize.

