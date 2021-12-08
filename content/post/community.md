+++
author = "Rasim"
comments = false
date = "2016-9-01"
draft = false
image = ""
menu = ""
share = false
slug = "community"
title = "5 - Finding Communities"
+++

As we are interested in analyzing the relations amongst the characters. In particular, we want to try to detect communities and study their characteristics. In order to perform this analysis, we are going to apply the Louvain Algorithm for community detection to the undirected network created previously.

![Community Distribution](/images/community.png)

The algorithm detects 5 small communities that have less than 10 characters, and 9 bigger communities that have between 20 and 50 characters.

In the following plot the network is represented with a different color for every community.

![Community Distribution 2](/images/community2.png)

The characters belonging to the 5 most populous communities have been reported below.

| Community 1             |       Community 2       | Community 3            |      Community 4       | Community 5               |
| ----------------------- | :---------------------: | ---------------------- | :--------------------: | ------------------------- |
| Alphinaud Leveilleur    |      Y'shtola Rhul      | Estinien Wyrmblood     |       G'raha Tia       | Noah van Gabranth         |
| Alisaie Leveilleur      |     Thancred Waters     | Regula van Hydrus      |      Tataru Taru       | Gerolt Blackthorn         |
| Y'shtola Rhul           |    Urianger Augurelt    | Buscarron Stacks       |      Cid Garlond       | Lina Mewrilah             |
| G'raha Tia              |  Krile Mayer Baldesion  | Foulques               |    Biggs and Wedge     | Adalberta Sterne          |
| Estinien Wyrmblood      |     Minfilia Warde      | Ywain Deepwell         |   Gaius van Baelsar    | Aldis                     |
| Krile Mayer Baldesion   |   Louisoix Leveilleur   | Zhai'a Nelhah          |    Nael van Darnus     | Deep Canyon               |
| Tataru Taru             |     F'lhaminn Qesh      | Lalai Lai              |    Livia sas Junius    | Leavold                   |
| Unukalhai               |        Unukalhai        | Waldeve                |   Midas nan Garlond    | Mylla Swordsong           |
| Biggs and Wedge         |       Emet-Selch        | Ysayle Dangoulain      |    Nero tol Scaeva     | Wide Gulley               |
| Igeyorhm                |        Elidibus         | Thordan VII            |  Rhitahtyn sas Arvina  | Brithael Spade            |
| Fordola rem Lupis       |        Lahabrea         | Alberic Bale           |   Vitus quo Messalla   | Khloe Aliapoh             |
| Regula van Hydrus       |        Igeyorhm         | Haldrath               |     Eline Roaille      | T'kebbe Morh              |
| Buscarron Stacks        |        Nabriales        | Heustienne de Vimaroix |        Bahamut         | Zhloe Aliapoh             |
| Foulques                |         Loghrif         | Lucia Junius           |         Tiamat         | Ejika Tsunjika            |
| Ywain Deepwell          |         Mitron          | Rasequin               |       Mide Hotgo       | Mikoto Jinba              |
| Pipin Tarupin           |  Niellefresne Thaudour  | Thordan I              |         Matoya         | Ramza Beoulve             |
| Ysayle Dangoulain       |     Severian Lyctor     | Hraesvelgr             |         Seiryu         | Alma Beoulve              |
| Thordan VII             |      Midnight Dew       | Nidhogg                |         Genbu          | Fran Eruyt                |
| Alberic Bale            | Fourchenault Leveilleur | Ratatoskr              |         Sophie         | Ashelia B'nargin Dalmasca |
| Haldrath                |         Ardbert         | Faunehm                |        Soroban         | Rasler B'nargin Dalmasca  |
| Heustienne de Vimaroix  |         Branden         | Orn Khai               |         Feo Ul         | Ba'Gamnan                 |
| Lucia Junius            |          Cylva          | Vedrfolnir             |         An Lad         | Eureka(primal)            |
| Rasequin                |         Lamitt          | Vidofnir               |        Ezel II         | Mutamix Bubblypots        |
| Thordan I               |        Nyelbert         | The Steps of Faith     |        Titania         | Alma bas Lexentale        |
| Hraesvelgr              |        Renda-Rae        | Midgardsormr           |        Tyr Beq         | Jenomis cen Lexentale     |
| Nidhogg                 |          Ryne           | Shiva                  |          Doga          | Ramza bas Lexentale       |
| Ratatoskr               |        Beq Lugg         | Ravana                 |          Unei          | Drake Rhodes              |
| Tiamat                  |        Lue-Reeq         | Knights of the Round   |     Ultima Weapon      | Jalzahn Daemir            |
| Faunehm                 |          Gaia           | Sephirot               |       Alexander        | Rowena                    |
| Orn Khai                |          Giott          | Sophia                 | Quickthinx Allthoughts | Bajsaljen Ulgasch         |
| Vedrfolnir              |         Granson         | Zurvan                 |   Cloud of Darkness    | F'hobhas                  |
| The Steps of Faith      |         Ran'jit         | Chieftain Moglin       |        Radovan         | Jihli Aliapoh             |
| Mide Hotgo              |         Lanbyrd         | Kazagg Chah            |         Omega          |                           |
| Midnight Dew            |         Olvara          | Lightning              |                        |                           |
| Fourchenault Leveilleur |          Seto           | Noctis Lucis Caelum    |                        |                           |
| Matoya                  |         Sul Oul         | Shantotto              |                        |                           |
| Seiryu                  |       The Twelve        | Garuda                 |                        |                           |
| Genbu                   |        Hydaelyn         |                        |                        |                           |
| Soroban                 |         Zodiark         |                        |                        |                           |
| Beq Lugg                |  Final Coil of Bahamut  |                        |                        |                           |
| Lyna                    |        Bismarck         |                        |                        |                           |
| Tesleen                 |       Hythlodaeus       |                        |                        |                           |
| Halric                  |         Sauldia         |                        |                        |                           |
| Chai-Nuzz               |         Tadric          |                        |                        |                           |
| Dulia-Chai              |                         |                        |                        |                           |
| Tristol                 |                         |                        |                        |                           |
| Feo Ul                  |                         |                        |                        |                           |
| Shiva                   |                         |                        |                        |                           |
| Bismarck                |                         |                        |                        |                           |
| Ravana                  |                         |                        |                        |                           |
| Sephirot                |                         |                        |                        |                           |
| Sophia                  |                         |                        |                        |                           |
| Zurvan                  |                         |                        |                        |                           |
| Alexander               |                         |                        |                        |                           |
| Susano                  |                         |                        |                        |                           |
| Lakshmi                 |                         |                        |                        |                           |
| Brayflox Alltalks       |                         |                        |                        |                           |
| Chieftain Moglin        |                         |                        |                        |                           |
| Ga Bu                   |                         |                        |                        |                           |
| Quickthinx Allthoughts  |                         |                        |                        |                           |

Characters belonging to the same community, are expected to be more connected to each other in the game compared to character belonging to different communities. To prove this point more accurately, it would be necessary to analyze the game more in deep and gather information regarding the actual story behind each character and their true relations with each other in the game. We will not continue this analysis. Instead, we are going to analyze which words are the most representative of each community and finally, we will study the average sentiment of these communities, to understand if there is a common positive or negative feeling among the character of a group.

#### 5.1 - Common words in the communities

We identified the most descriptive words related to each community. The objective is to understand if different communities have different related words. We used two different methods: the TF and and the TF-IDF. The first one will take into account how much a specific word appear in the text, while the other will also consider how often that word appear through the whole database, adding value to those words that are more characteristic of a specific community, therefore more relevant.

The most common words using TF for the top 5 communities are like given below:

| Alisaie Leveilleur's community | Estinien Wyrmblood's community | Warrior of Light's community | Alphinaud Leveilleur's community | Edmont de Fortemps's community |
| ------------------------------ | ------------------------------ | ---------------------------- | -------------------------------- | ------------------------------ |
| man                            | garuda                         | yoshida                      | ga                               | marcelloix                     |
| woman                          | final                          | naoki                        | bu                               | character                      |
| player                         | fantasy                        | final                        | alisaie                          | final                          |
| hyuran                         | messenger                      | fantasy                      | kobold                           | fantasy                        |
| imp                            | xv                             | april                        | final                            | ehll                           |

The most common words using TF-IDF for the top 5 communities are like given below:

| Alisaie Leveilleur's community | Estinien Wyrmblood's community | Warrior of Light's community | Alphinaud Leveilleur's community | Edmont de Fortemps's community |
| ------------------------------ | ------------------------------ | ---------------------------- | -------------------------------- | ------------------------------ |
| woman                          | garuda                         | yoshida                      | alisaie                          | marcelloix                     |
| hyuran                         | messenger                      | naoki                        | kobold                           | ehll                           |
| imp                            | wind                           | april                        | titan                            | francel                        |
| unsavory                       | xv                             | fool                         | warrior                          | family                         |
| nero                           | statue                         | director                     | bu                               | craftsman                      |

It appear clear how the TF-IDF analysis gives more interesting results in identifying the most relevant words of a community, by eliminating recurring words as 'fantasy', 'player' and 'final' that are clearly related to the game itself, and thus very common in all the communities. We can also see from the results that the second method does not ever return the same word for different communities, as it happen in the TF analysis, confirming that the TF-IDF is more accurate in detecting the relevant words in a community.
