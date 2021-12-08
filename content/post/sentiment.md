+++
author = "Rasim"
comments = false
date = "2016-9-01"
draft = false
image = ""
menu = ""
share = false
slug = "sentiment"
title = "6 - Sentiment Analysis"
+++

We now proceed performing a sentiment analysis of the communities, after we gather the adequate text information related to the story of the characters.

We are going to perform different analyses. Firstly, we are going to use the LabMT dataset, to calculate the sentiment of each token, created from the textual description of the characters obtained from the wikipages, after proper tokenization and lemmatization. Subsequently, we are going to repeat the same process, this time using the text obtained from written dialogues extracted from the game. This second analysis is expected to return a better understanding of the sentiment of the characters, since it will contain more textual information related to the feelings and sentiments of the characters during the game.

Lastly, we will use the VADER sentiment analysis tool, applied on the dialogues text. This method will also take into account different aspects of the speeches, like the use of punctuation, capital letters and specific expressions.

#### 6.1 - Sentiment Analysis 1

**Data**: Text description from the Wikipages

**Method**: LabMT

![Sentiment Distribution](/images/sentiment-distribution.png)

All values are just above 5, showing that there is a slight positive sentiment, althogh since the text used for this analysis was collected from the descriptions of the characters, the information they carry about feelings and sentiments of the characters is quite poor, hence the result is expected. We now repeat the analysis with a more relevant database: written dialogues from the videogame.

#### 6.2 - Sentiment Analysis 2

**Data**: Dialogues from the Videogame

**Method**: LabMT

![Average Sentiment](/images/average-sentiment.png)

As a result, all values are all between the value 5 and 6, meaning there is a slight positive average sentiment in all communities. The error bars do not show a great variance in the values, meaning that the character in every community take all similar values. We now proceed with the VADER analysis, using the Dialogue dataset.

#### 6.3 - Sentiment Analysis 3

**Data**: Dialogues from the Videogame

**Method**: VADER

![Average Sentiment Vader](/images/average-sentiment-vader.png)

The VADER analysis gives more interesting results. All communities scored a value greater than zero, that means the average sentiment is positive, in particular, the Warrior of Light (Final Fantasy XIV) 's community, scored 0.869, meaning a great positivity in the text. In this case we can also see from the error bars that there is much more variance in the characters of one community. For example, the Lyse Hext 's community scored the positive value 0.636 even though the error bars indicate at least one character got a negative result.
