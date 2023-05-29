# Machine Learning to predict Sentiments

- The Machine Learning Algorithm that we'll use to combine all the things (cleaning of text, text to numerical value) will be **NaiveBayes Classifier**
  > NaiveBayes tends to be the baseline model for every sentiment analysis task

## How our algorithm works?

![Bayes' Theorem](DOC_IMAGES/bayes-theorem.png)

- It finds out the probabilities of the classes assigned to the text by using the join probabilities of words and classes.
- `P(A/B)`: conditional probability of event A given event B. (prob of event A occuring given event B has occured)
- `P(B/A)`: conditional probability of event B given event A.
- `P(A)`: prior probability of event A. It represents the initial or prior belief in the probability of event A occuring.
- `P(B)`: prior probability of event B. It represents the initial or prior belief in the the prob. of event B occuring

### What we'll use

- Given the feature vector _(x1, ..., xn)_ and the class **Ck**, Bayes theorem is stated mathematically having the following relationship.

![Bayes' Theorem](DOC_IMAGES/modified-bayes-theorem.png)

### **Assumption our algorithm makes**

- One event in a class should be independent of another event belonging to the same class. (fact it assumes)
- The algorithm also assumes that the **predictors have an equal effect on the outcomes or responses in the data**.

### Various vairants

1. Gaussian Naive Bayes
2. Bernoulli Naive Bayes
3. Multinomial Naive Bayes (we'll use this)

   [Learn more about the variants](https://www.analyticsvidhya.com/blog/2022/03/gaussian-naive-bayes-algorithm-for-credit-risk-modelling/#:~:text=In%20Gaussian%20Na%C3%AFve%20Bayes%2C%20the,are%20calculated%20for%20each%20class)
