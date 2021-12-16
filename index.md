![](./docs/networking-vs-connecting.jpg)

## Introduction 

It is very often the case that well-known personalities are quoted in speeches given by other individuals, creating a directional relationship from a speaker to a subject. These relationships occur between two persons with different characteristics, for example their occupation and their gender. As a result, these relationships can be multiple with (very) different natures, where some of these are perhaps more present than others.

This brings us to the question, how are these relationships distributed? In this article, we propose to study and understand the relationships between several individuals according to the occupation and gender of each person involved in a relationship. To do so, we want to establish a directed graph of relationships between speakers and people mentioned in the quotations. In particular, some of the questions that will be answered in this article are:

* Are these relationships uniform, i.e., involving people of the same occupation?
* How are the genders represented according to occupation in each relationship?
* Are these relationships likely to change over time?


## The data

In this study we use the Quotebank dataset, a dataset of 178 million unique, speaker-attributed quotations that were extracted from 196 million English news articles crawled from over **377 thousand web domains** between August 2008 and April 2020. We will focus on the years of **2015 to 2020**. 

Using SpaCy, we extract 100 000 quotations for each year (2015 to 2020) in which a speaker is talking about a human subject. After cleaning, we get the following amount of samples:


| Year | Number of quotations | Number of speakers | Number of subjects |
| --- | --- | --- | --- |
|2015|15970|8146|6060|
|2016|17392|7966|5814|
|2017|16389|8177|6009|
|2018|16111|7985|6063|
|2019|15946|7530|5583|
|2020|17498|7000|5274|


## How are the genders represented ? (Question 2)

We now want to look at what this data tells us about gender equality. Do men, women and other genders are the same visibility in the media in general?

 |
:--- | --- :
|<img src="./docs/Gender_speakers.png " alt="Forest"> |<img src="./docs/Gender_subjects.png " alt="Forest">|





Subsequently, we select additional variables to use for a meaningful clustering. We present the found relationships between speakers and referred persons on a graph, whose nodes the clusters and edges represent the “has mentioned” relationship.

## Some occupations are at the heart of the relationships…

Test here 
Is it working? Yes

{% include Gender_speakers.html %}

<iframe width="760" height="1155" src="./docs/Gender_speakers.html"></iframe>

## … and often very gendered ones.

Below is the same graph than before but this time with the occupation and gender of each person as a comparison key.

## Towards an evolution in time?

