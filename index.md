![](./docs/networking-vs-connecting.jpg)

## Introduction 

It is very often the case that well-known personalities are quoted in speeches given by other individuals, creating a directional relationship from a speaker to a subject. These relationships occur between two persons with different characteristics, for example their occupation and their gender. As a result, these relationships can be multiple with (very) different natures, where some of these are perhaps more present than others.

This brings us to the question, how are these relationships distributed? In this article, we propose to study and understand the relationships between several individuals according to the occupation and gender of each person involved in a relationship. To do so, we want to establish a directed graph of relationships between speakers and people mentioned in the quotations. In particular, some of the questions that will be answered in this article are:

* Are these relationships uniform, i.e., involving people of the same occupation?
* How are the genders represented according to occupation in each relationship?
* Are these relationships likely to change over time?


## Preliminary analysis

Using SpaCy, we extract 100 000 quotations for each year (2015 to 2020) in which a speaker is talking about a human subject. After cleaning, we get the following amount of samples:

(TO DO pretty)

| Year | Number of quotations | Number of speakers | Number of subjects |
| --- | --- | --- | --- |
|2015|     |     |     |
|2016|     |     |     |
|2017|     |     |     |
|2018|     |     |     |
|2019|     |     |     |
|2020|     |     |     |


We then make a preliminary analysis on the extracted names and their gender and occupation distribution. Here

<iframe width="760" height="1155" src="./docs/Gender_speakers.html"></iframe>

Subsequently, we select additional variables to use for a meaningful clustering. We present the found relationships between speakers and referred persons on a graph, whose nodes the clusters and edges represent the “has mentioned” relationship.

## Some occupations are at the heart of the relationships…

Test here 
Is it working? Yes

<iframe width="760" height="1155" src="./docs/nt.html"></iframe>

## … and often very gendered ones.

Below is the same graph than before but this time with the occupation and gender of each person as a comparison key.

## Towards an evolution in time?

