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

We tried to find the most important words related to each affiliation using both TF and TF-IDF. Below we reported the results for the 3 greatest affiliation:

> Garlean Empire, High Houses of Ishgard, Doma

#### 4.1 - Word Clouds

|                                            |                                            |                                      |
| ------------------------------------------ | ------------------------------------------ | ------------------------------------ |
| ![Garlean Wordcloud](/images/garlean1.png) | ![Ishgard Wordcloud](/images/ishgard1.png) | ![Doma Wordcloud](/images/doma1.png) |

![Wordcloud](/images/wordcloud2.png)
