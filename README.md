# Fake-news-detector
A project to detect whether a given piece of news is fake or not.
It used Passive aggressive classifier - an ML algorithm which classifies a given tweet as either Passive(real) or Aggressive(fake). For this purpose we have a labelled data with the following columns
Id number - used to identify the news
title - The title of the news
text - the full text of the news
label - stating whether the given news is real or fake

With this we split the data as training and test set. We convert the given text using tf-idf vectorizer 
TF (Term Frequency): The number of times a word appears in a document is its Term Frequency. A higher value means a term appears more often than others, and so, the document is a good match when the term is part of the search terms.

IDF (Inverse Document Frequency): Words that occur many times a document, but also occur many times in many others, may be irrelevant. IDF is a measure of how significant a term is in the entire corpus.

The TfidfVectorizer converts a collection of raw documents into a matrix of TF-IDF features.

The model that we used for classifying the text is Passive Aggressive Classifier
Passive Aggressive algorithms are online learning algorithms. Such an algorithm remains passive for a correct classification outcome, and turns aggressive in the event of a miscalculation, updating and adjusting. Unlike most other algorithms, it does not converge. Its purpose is to make updates that correct the loss, causing very little change in the norm of the weight vector.

Then we test our model using our test data. We are having an accuracy of 92%
