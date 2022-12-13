---
title: "Network Analysis Practice: Flying Team"
date: 2022-04-07T21:53:20.415Z
draft: false
featured: false
authors:
  - admin
tags: 
  - Data Visulization
  - Newworks
image:
  filename: cover.webp
  focal_point: Smart
  preview_only: false
  caption: "Photographer: M. McNeil, for Fox Photos. Images courtesy of the Hulton
    Archive/ Getty Images. Colorized and researched by Benjamin Thomas, Photo
    Source:
    [link](https://www.vintag.es/2015/05/50-breathtaking-wwii-photos-look-like.\
    html)"
---
## Introduction

Network analysis has been a practical technique since the 1930s. It has had a great impact on the social sciences, computer graphics, and physics. In essence, networks can be found in all kinds of data, and their potential is becoming increasingly important in customer behavior analysis, and social media analysis in the digital age. I chose to follow the social sciences to learn and practice my skills in network analysis and visualization, because most of the fundamental theories and principles were developed by social scientists, and this approach will help me to have a more solid understanding of this technique in order to further apply my knowledge to other disciplines.

The data used in this project is get from the Center for Computational Analysis of Social and Organizational Systems (CASOS). The data was collected in 1943 by Leslie D. Zeleny from a test of forty-eight cadet pilots at a US Air Force flying school. The test participants were asked to fill out a questionnaire to name who they would like to fly with and who they would not like to fly with after randomly partnered with another for flying training.

The data set comes with two parts in a single .xml file, with 48 nodes representing the cadet pilots and 357 directed edges representing their responses to the questionnaire.

## Inspiration

I didn’t find other visualizations based on the same datasets. However, the Exploratory Social Network Analysis with Pajek comes with some analytical network graphs for affective relations gave me some ideas.

![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/04/affective_relations_graph.png?resize=741%2C447&ssl=1)

Sociogram Example From Exploratory Social Network Analysis with Pajek, ch4, Figure 4.5

The example uses data collected from a company that shows sentiments among colleagues. The positive affections are labeled with solid lines and the negative affections are labeled with dashed lines. Negative edges are also used as partitions that distinguish clusters. The number in nodes shows groups, it is worth noting that groups and clusters are not equivalent in this graph since negative affections inside a cluster are less important than those between clusters, and cycles (mutual affections) are highlighted for further study.

This graph is quite understandable in an academic paper, but not quite readable to general audiences. It gives me a solid start on sociograms to develop my visualization work.

### Software

#### Gephi

I employed Gephi to make my network visualization. Gephi is an open-source software for creating network graphs. It requires some data cleaning work in advance. I’ll talk more about the process in the next section.

#### Adobe Illustrator

Adobe Illustrator is one of the most powerful image editing software right now. I have done the final graph editing with it.

## Process

### Data Cleaning

The first step of all is to separate the nodes and the edges datasets from the .xml file. I used Openrefine to do this and saved them in two .csv files ready to be sent to Gephi for visualization. However, I noticed that Gephi only gives the total in- and out- degrees for a node. It does not show the positive or negative numbers highlighted. Thus, I employed R Studio to calculate the sum value of in-degree (1 for positive and -1 for negative) for each node that reflects the pilot’s overall popularity among the flying team.

### Clustering

I spent a lot of time finding a clear partition to create clusters and I finally realize that my data set is not clusterable as there are too many edges among the relatively small number of nodes. Thus, I decided to make two graphs, each focusing on the positive edges and negative edges respectfully. I then manually arranged the nodes as a semi-circle and finally merged them with Illustrator. The color of each node distinguishes its sentiment. Green represents positive and violet represents negative. The saturation of each node represents its in-degree. For example, node c13 received the most positive votes and node c26 received the most negative votes.

![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/04/POS_NEG_CLASTER-889x1024.png?resize=532%2C613&ssl=1)

Positive and Negative Clusters based on sentiment

## Result

![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/04/Artboard-1-1024x576.png?resize=840%2C473&ssl=1)

## Reflection

In the process of using Gephi for visualization, I noticed the limitations of my dataset. First, unlike thematic datasets or other types of statistics, social relationship data does not inherently lend itself to combinations of small numbers of nodes and large numbers of edges. It is difficult to cluster such data in the visualization results. I continued to experiment with other layouts and finally created the following visualization to help readers understand the distribution of data more intuitively.

![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/04/flyingTeams_4.png?resize=840%2C268&ssl=1)

## **References**

* J. L . Moreno (et al.), The Sociometry Reader (Glencoe (Illinois): The Free Press, 1960, p. 534-547).
* W. de Nooy, A. Mrvar, and V. Batagelj, Exploratory Social Network Analysis with Pajek (Cambridge: Cambridge University Press, 2004), Chapter 4.

<!--EndFragment-->