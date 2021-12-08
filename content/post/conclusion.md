+++
author = "Rasim"
comments = false
date = "2016-8-01"
draft = false
image = ""
menu = ""
share = false
slug = "conclusion"
title = "7 - Conclusion"
+++

We analyzed Final Fantasy XIV's character descriptions and dialogue in this project. After data extraction and preprocessing using the Final Fantasy Fandom Wiki's API and regular expressions, a directed network was built and found to be behaving as a sparse, scaled-free network. The most linked characters met our expectations based on knowledge of the game, as they are central characters with a significant influence on the plot and the outcomes of the game.

The communities found through the Louvain Algorithm have different relevant words, calculated using the TF-IDF algorithm, which could be caused by differences in the plot of the story for those groups of characters. The following sentiment analysis enabled us to study the positivity of the communities, and the differences of sentiment between the text descriptions of the characters and actual dialogues from the game. Using the LabMT database, the sentiment analyses resulted in a mild positive sentiment, both for the text description and for the dialogues, meaning either the words collected from the texts could not transpares the real feelings or the characters truly had a rather neutral sentiment. More interesting results were achieved through the VADER algorithm, that adding the punctuation to the analysis and studying the meaning of the whole sentences rather than the single words, managed to obtain a more realistic description of the feeling in the communities, although with higher variance amongst the characters.

The analyses could be improved by adding more information for every character, for example more dialogues, or more backstories. In this way we would be able to better analyze the sentiment of each character and also create more accurate communities, that could be based on their characteristics instead of their connections. For the purpose of this project however, we are satisfied with the knowledge we managed to gather by studying the information that we had about the game, its characters and the their relations.
