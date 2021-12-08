+++
author = "Rasim"
comments = false
date = "2016-10-01"
draft = false
image = ""
menu = ""
share = false
slug = "network"
title= "3 - Network"
+++

The network created contains 385 nodes, each one related to character and 1472 edges. Firstly, we discarded the isolated nodes resulting in 335 remaining nodes. Afterwards, we extracted the Giant Component obtaining the final network which has 320 nodes and 1449 links.

| ![Network](/images/network.png) |
| :-----------------------------: |
|  _FFXIV (Undirected) Network_   |

While there are significant hubs, the network is not dominated by a single entity. It is expected that in an online RPG, the protagonist is not as critical to the game's plot development relative to single-player games.

#### 3.1 - Network Analysis

Studying the in-degree we found that the 5 most connected characters are:

1. Alphinaud Leveilleur(57)
2. Gaius van Baelsar(37)
3. Y'shtola Rhul(35)
4. Zenos yae Galvus(35)
5. Thancred Waters(34)

Analyzing the out-degree we can see that the 5 most connected characters are:

1. Alphinaud Leveilleur(33)
2. Lyse Hext(30)
3. Y'shtola Rhul(26)
4. Elidibus(25)
5. Thancred Waters(22)

Alphinaud Leveilleur is the most connected character both in the in-degree and out-degree sets. He is a significant character in the game. It might be surprising that the main character is not the most connected one, but it is sensible in the context of the dataset: the protagonist of the game is silent. Typically in such plots, a companion character is talkative and well-connected. This is to minimize boredom and break the monotone of silence in the game.

The plots of the degree distributions are reported below.
| | |
| ------------------------------------------ | ------------------------------------------ |
| ![In-Degree Distribution](/images/in-degree.png) | ![Out-Degree Distribution](/images/out-degree.png)|

In-Degree distribution shows that only a few characters have a degree higher than 25, while the great majority of them are between 0-10.

Out-Degree distribution shows a similar behaviour with the majority of the nodes below a degree of 10.

Graphically, the in-degree distribution appears to follow a power law distribution, indicating a scale-free network (real network). The out-degree distribution seems to follow a power law distribution, but it is less skewed to the right, and is more difficult to interpret.

We use the powerlaw function below to fit a power distribution and get the gamma values for further analysis.

|                                              |                                               |
| -------------------------------------------- | --------------------------------------------- |
| ![In-Degree Powerlaw](/images/powerlaw1.png) | ![Out-Degree Powerlaw](/images/powerlaw2.png) |

For the in-degree distribution, the exponent value (γ=2.33) indicates that the network is in the scale-free regime (ultra-small world). As for the out-degree distribution, the exponent is almost equal to the critical value of 3 (γ=3.01). While this makes the out-degree distribution more random-like, it is still not the same as a random network, for the value indicate the presence of a double logarithmic correction _lnlnN_ which shrinks the distances of this network relative to a random network.

We will compare our network below to a random one of the same probability for further confirmation.

|                                       |                                                         |
| ------------------------------------- | ------------------------------------------------------- |
| ![Random Network](/images/random.png) | ![Degree Distribution of Wiki](/images/degree-dist.png) |

As seen above, the network's degree distribution significantly deviates from the expected random network. Our graphical, power-law and random network comparison are thus in agreement.
