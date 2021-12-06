+++
author = "syui"
comments = false
date = "2016-10-01"
draft = false
image = ""
menu = ""
share = false
slug = "network"
title= "Network"
+++

The network created contains 385 nodes, each one related to character and 1472 edges. Firstly, we discarded the isolated nodes resulting in 335 remaining nodes. Afterwards, we extracted the Giant Component obtaining the final network which has 320 nodes and 1449 links.

| ![Network](/images/network.png) |
| :-----------------------------: |
|  _FFXIV (Undirected) Network_   |

#### Network Analysis

Studying the in-degree we found that the 5 most connected characters are Alphinaud Leveilleur(56), Gaius van Baelsar(37), Y'shtola Rhul(35), Thancred Waters(34), Zenos yae Galvus(33).

Analyzing the out-degree we can see that the 5 most connected characters are Alphinaud Leveilleur(33), Lyse Hext(30), Y'shtola Rhul(26), Elidibus(25), Thancred Waters(22).

The plots of the degree distributions are reported below.
| | |
| ------------------------------------------ | ------------------------------------------ |
| ![In-Degree Distribution](/images/in-degree.jpeg) | ![Out-Degree Distribution](/images/out-degree.jpeg)|

In-Degree distribution shows that only a few characters have a degree higher than 25, while the great majority of them are between 1-10.

Out-Degree distribution shows a similar behaviour with the majority of the nodes below a degree of 10.

<!--
Powerlaw, random network should be added
-->
