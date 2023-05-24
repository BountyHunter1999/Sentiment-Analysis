# Cleaning the data

[Sentiment Analysis on Movie Reviews](https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/data)

1. [Tokenization](#1-tokenization)
2. [Converting the text from upper case to lower case](#2-converting-the-text-from-upper-case-to-lower-case)
3. [Correcting the spelling mistakes](#3-correcting-the-spelling-mistakes)
4. [Punctuation removal]()
5. [Number removal]()
6. [Stop words removal]()
7. [Normalization via lemmatization or stemming]()

# 1. Tokenization

- Tokenization is a way to split the strings into a list of words
- Types:
  i. One that convert the whole sentence into a list of sentences
  ii. Convert the strings into separate words (tokens)

> We can use regex to tokenize but it is a bit difficult although it gives more control over the text

# 2. Converting the text from upper case to lower case

- Hello -> hello
- HELLO -> hello

# 3. Correcting the spelling mistakes

- We should always check for misspellings in the list so the model performs well
  > GIGO, Garbase In Garbage Out
- the drawback of using something like Speller from AutoCorrect is that it's really slow. (So ignore this step if slow pc😉)
