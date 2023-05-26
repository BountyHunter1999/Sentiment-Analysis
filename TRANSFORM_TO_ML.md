# Transforming Text Data to a form a Machine Learning Model Understands

- Since ML models doesn't understand textual data we need a way to convert the data we obtain after cleaning the text data into some numeric form so that it can be fed into the model so that it can perform some form of computations on it.

we can use 2 main tools

1. CountVectorizer
2. TF-IDF

## 1. CounterVectorizer

- CountVectorizer is a great feature extraction tool provided by sklearn.
- It's basic purpose is that it **converts a given text into a vector-based on the count(frequency) of the occurence of each word in a list.**
- It creates a sparse matrix of the count of the numbers.
`from sklearn.feature_extraction.text import CountVectorizer`
