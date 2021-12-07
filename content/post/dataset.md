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

Our dataset consists in the characters' wikis obtained from [Final Fantasy Fandom Wikipages](https://finalfantasy.fandom.com/wiki/Final_Fantasy_XIV_characters).

If you want to download the files containing the characters data [click here](https://finalfantasy.fandom.com/wiki/Final_Fantasy_XIV_characters). (You will have access to a zip file containing a .txt file for each characters of the wiki.)

To perform sentiment analysis, we've also used [a dialogue collection](https://docs.google.com/document/d/1wlFBfhu7wjHlMEVSEZgEHpaaJIQBhrmh-RIdWYGMJZM/edit).

From each character wikipage we obtained the information related to age, race, gender, affiliation and occupation using regular expressions. Then we used this information to create a dataframe of 385 different characters. Afterwards, we searched the pages for links to other characters and created the network.
