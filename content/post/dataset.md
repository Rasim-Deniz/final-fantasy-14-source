+++
author = "Rasim"
comments = false
date = "2016-11-01"
draft = false
image = ""
menu = ""
share = false
slug = "dataset"
title= "2 - Dataset"
+++

We analyzed two datasets for Final Fantasy XIV:

- ##### The fan wiki of Final Fantasy XIV

The **_[Final Fantasy XIV's wiki](https://finalfantasy.fandom.com/wiki/Final_Fantasy_XIV_characters)_** was used to download all characters' descriptions and attributes.

The data was extracted using the fandom wiki's API and stored in JSON. Regular expressions were utilized to extract the description of each character along with the attributes of interest: race and affiliation. Other attributes were also extracted: gender, age, and occupation.

If you want to download the files containing the characters data **_[click here](/project/files/ff14_chars_json.zip)_**. (You will have access to a zip file containing a .txt file for each characters of the wiki.)

- ##### The game's dialogue

All the **_[dialogue between characters](https://docs.google.com/document/d/1wlFBfhu7wjHlMEVSEZgEHpaaJIQBhrmh-RIdWYGMJZM/edit)_** was obtained for text and sentiment analysis to explore the game's characters world through text interactions.

#### 2.1 - Data Preprocessing

Our strategy was to use regular expressions that have more false positives than false negatives and then clean the edge cases manually based on our knowledge of the dataset. The following data preprocessing was performed:

- **Duplicates Removal**: Some characters are referred to using different names in the wiki. This was detected and fixed by keeping only the unique characters.
- **Redirects Handling**: The redirects were detected using a regular expression, then the correct character pages were manually hard-coded to refer to the right link
- **Class Re-Assignment**: Some classes have different synonyms. For instance, the race "hume" is the same as "hyur." This was fixed by re-assigning the same categories in such cases.
- **Regex Fixing**: Edge cases in which our regular expressions obtained false positives and negatives were fixed manually by assigning the false values to the correct ones.

For text analysis, the following was done:

- **Removal of stop words and punctuation**: Common stop words and punctuation were deleted so that the text analysis is not influenced by it
- **Tokenization and lemmatization**: The text was tokenized and lemmatized in the dialogue and for each character.

#### 2.2 - Data Statistics:

Number of characters: _**385**_

Total Data size: _**3.21 MB**_

Number of links (Directed): _**1477**_

Number of links (Undirected): _**1131**_

Most common characters (in-degree): Alphinaud Leveilleur, _**56**_

Most common characters (out-degree): Alphinaud Leveilleur, _**33**_
