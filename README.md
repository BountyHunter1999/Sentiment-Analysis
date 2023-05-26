# Cleaning the data

[Sentiment Analysis on Movie Reviews](https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/data)

1. [Tokenization](#1-tokenization)
2. [Converting the text from upper case to lower case](#2-converting-the-text-from-upper-case-to-lower-case)
3. [Correcting the spelling mistakes](#3-correcting-the-spelling-mistakes)
4. [Punctuation removal](#4-remove-punctuations)
5. [Number removal](#5-remove-numbers)
6. [Stop words removal](#6-remove-the-stopwords)
7. [Normalization via lemmatization or stemming](#7-normalization)
   a. [Stemming](#i-stemming)

## 1. Tokenization

- Tokenization is a way to split the strings into a list of words
- Types:
  i. One that convert the whole sentence into a list of sentences
  ii. Convert the strings into separate words (tokens)

> We can use regex to tokenize but it is a bit difficult although it gives more control over the text

## 2. Converting the text from upper case to lower case

- Hello -> hello
- HELLO -> hello

## 3. Correcting the spelling mistakes

- We should always check for misspellings in the list so the model performs well
  > GIGO, Garbase In Garbage Out
- the drawback of using something like Speller from AutoCorrect is that it's really slow. (So ignore this step if slow pc😉)

## 4. Remove punctuations

- They oftern don't carry any meaning to the sentiment analysis

## 5. Remove numbers

- Numbers typically don't contain much information.
- In some datasets, they might but in the dataset we're looking it doesn't

## 6. Remove the stopwords

- Stopwords are those irrelevant words, which do not contain much meaning and do not help much in sentiment analysis.
  eg.
  > `["i", "me", "my", "myself", "we", "our", "ours", "ourselves", "you", "you're", "you've", "is", "the", "a"]`
- we can remove them using stopwords in nltk

## 7. Normalization

- 2 common and famous techniques for Normalization:
  i. Stemming
  ii. Lemmatization

- In English language, a single word can take many forms as per the usage, such as assign, assigns, assigned, assigning, etc. When we tokenize, they refer to different words, but we know that they all share a common meaning.

### i. Stemming

- Stemming referes to the process of normalization, where we **reduce a word to its base stem**, for example, "automate", "automatic", "automation", "automations", will be reduced to "automat" such that all these forms refer to automat

### ii. Lemmatization

- It refers to doing things properly with the use of a vocabulary and morphological _(relating to form or structure of things)_ analysis, normally aiming to remove inflectional _(relating to or involving a change in the form of a word to express a grammatical function or attribute)_ endings only and to return the dictionary form of a word.

- This returns the dictionary or lemma format and contains more meaning
