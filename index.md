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

&nbsp;


## Some occupations are at the heart of the relationships… (Part 1)

Below is integrated a directed graph of relationships between speakers (people who mentioned someone) and subjects (people who have been mentioned) with the occupation of each person as a comparison key. In other words, a node corresponds to an occupation and a directed edge to the relations between these nodes, i.e., which occupation spoke to which occupation. The present entities (nodes and edges) are weighted according to their redundancy in the graph. Two nodes are close if the relation between these two nodes is strong, i.e., the weight of the edge is large (also nodes and edges are darker). The graph is interactive, feel free to zoom or select nodes!

<iframe src="./docs/nt_occupation_2015.html"  width=800 height=1200 id="graph1"></iframe>



Analysis : relashionships ~ 2 paragraph 



## … and often very gendered ones. (Part 2)

Below is a directed graph represening the interactions between speakers and subjects but this time the graph is generated with the occupation and gender of each person as a comparison key. Nodes and edges in blue and red concern respectively males and females.

<iframe src="./docs/nt_2015.html"  width=800 height=1200 id="graph2"></iframe>

Compared to the graph with the occupation as a comparison key, 2 clusters are clearly visible : the "female cluster" and the "male cluster". Both are very connected within themselves, very far apart from each other and highlight several differences between males and females. 

Whether one is a male or a female, occupations are not distributed in the same way, where as an example, sportswomen are not represented, hence a smaller number of nodes. Note also that men are more present in some occupations than women, as for example in politics. 

Especially, the female’s cluster could be separated in such a way that females are gathered in the field of art (singers for example) or in the humanities (politicians for example), where these areas are distant from each other. As for the relationships between women, they communicated mainly between domains, where the politicians and lawyers do not communicate with people of the artistic field. On top of everything else, singers and actors seem to be at the heart of the attention, being the occupations that most women refer to.

About males, they are much more represented and especially in different occupations ! Science and sport as occupations are very present compared to females, as well as religion. (TODO: continue)

Finally, what about relationships between males and females ? Well, almost none… The graph shows a real separation and gap in communication between them where it is mostly the people attached to the public domain who are closest to the men. The artistic field does not escape it, where women don’t communicate much with men, even in the same field. On the whole, relationships between individuals are very gendered ones according to the occupation that each one occupies. 

---------------------------------------------------------

Now what the data tells us about the visibility of men, women and other genders in the media in general according to their occupation?

Below is a directed graph represening the interactions between speakers and subjects but this time the graph is generated with the occupation and gender of each person as a comparison key. Nodes and edges in blue and red concern respectively males and females.

<iframe src="./docs/nt_2015.html"  width=800 height=1200></iframe>

Compared to the graph with the occupation as a comparison key, 2 clusters are clearly visible : the "female cluster" and the "male cluster". Both are very connected within themselves, very far apart from each other and highlight several differences between males and females. 

At first we can see that the female and male clusters have very different sizes. And if we take a closer look on the data we can see that, indeed, women are very underrepresented in the media.

 |
:--- | --- :
|<img src="./docs/Gender_speakers.png" alt="Forest"> |<img src="./docs/Gender_subjects.png " alt="Forest">|

According to worldometers in 2013 there are 50.4 % of men and 49.6 % of women  in the world. Hence it seems that women are very underrepresented in the media. Indeed **women are the origin of less than 20 % of the quotes** that are reported in the media and are **5 times less likely than men to be spoken** about in the media.

We now have a closer look at the graph and want to know what are the occupations of the women represented in the media compared to men.

Let's start with the women occupations.

Most of the women present in the media are artists. There is also a few politicians.
We notice that although on repartition quite a lot of women which said quotes are involved in politics (throughout the years  always more than 17%) or are researchers, business persons, most of the women names found in quotes are artists. And women politicians are way more represented as speakers than as subjects. 

Now what about the men occupations?

Most of the men present in the media are politicians, artists and sports players. They are much more represented than female in the different occupations and especially in science and sport as well as religion. 


Finally, what about relationships between males and females ? Well, almost none… The graph shows a real separation and gap in communication between them where it is mostly the people attached to the public domain who are closest to the men. The artistic field does not escape it, where women don’t communicate much with men, even in the same field. On the whole, relationships between individuals are very gendered ones according to the occupation that each one occupies. 
Is it really that men only talk about other men and women only talk about other women?

We provide the following graph:

{% include Gender_link_subjects.html %}

In fact we can see that in general a women is 3 times more likely that a men to speak about another women. Now let's see what happens if we focus on an occupation in particular.

\\
\\

## Towards an evolution in time? (Part 3)

Evolution







