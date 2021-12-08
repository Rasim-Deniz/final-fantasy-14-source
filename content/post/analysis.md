+++
author = "Rasim"
comments = false
date = "2016-9-01"
draft = false
image = ""
menu = ""
share = false
slug = "analysis"
title= "4 - Text Analysis"
+++

In order to perform the text analysis, we decided to prepare the data by applying tokenization and lemmatization to the character descriptions obtained from the wikipages.
Words related to the structure of the wiki and not to a specific character of the story, where also removed from the text.

The frequency distribution of the 75 most common tokens is reported below.
![Frequency Distribution](/images/frequency-words.png)

The frequency plot of the most common words is as expected: the two most common words are "final" and "fantasy," followed by "warrior" and "light." It is worth mentioning that the main character of the game is named "The Warrior of Light." Therefore, the high frequency of these two words is unsurprising.

#### 4.1 - Word Clouds

Word clouds are a visual representation of text data, typically used to depict keyword metadata (tags) on websites, or to visualize free form text. In this case, the tags are single words, and the importance of each tag is shown with font size: bigger term means greater weight.

**Goal:** Analyze the word cloud for some groups of characters

**Strategy:**

- Obtain the 3 greatest Affiliations, and the characters who belong to them.
- Calculate the TF and TF-IDF values for each affiliation
- Analyze the wordcloud over the text previously obtained.

The greatest Affiliations are:

> Garlean Empire 16
>
> High Houses of Ishgard 10
>
> Doma 9

The output of the wordclouds we obtained are given below.

![Wordcloud](/images/wordcloud2.png)
