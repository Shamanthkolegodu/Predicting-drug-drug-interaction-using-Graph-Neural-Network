# Predicting drug-drug interaction using Graph Neural Network


## Introduction
* Drug-Drug interaction is one of the most sought out areas due to its immense relevance.
* It is defined by the reaction between two or more drugs when in contact with one another. These interactions can either be supportive, or might lead to hazardous consequences.
* The use of graph neural networks instead of traditional manual techniques not only makes the process more efficient, but also helps in enhancing the accuracy by including connections that would not have been seen by manual approaches.
* We aim to build graph based link predictions and generate a comparative study of the same.

## Dataset
* Ogbl–ddi from Open Graph Benchmark 
    - Nodes - 4267
    - Edges - 13,34,889
* It is a homogenous, undirected, unweighted graph
representing drug-drug interactions. 
* Source- [link](https://ogb.stanford.edu/docs/linkprop/#ogbl-ddi)

## Overall design or approach in a free hand diagram

![alt text](https://github.com/Shamanthkolegodu/Predicting-drug-drug-interaction-using-Graph-Neural-Network/blob/main/Images/Design.png)

## Final results
* Metric :
    - Loss - BCEWithLogitsLoss
    - Accuracy
    - Hits : On validation set
    ![alt text](https://github.com/Shamanthkolegodu/Predicting-drug-drug-interaction-using-Graph-Neural-Network/blob/main/Images/table.png)

* Hits@100 for test dataset for various models
    - ![alt text](https://github.com/Shamanthkolegodu/Predicting-drug-drug-interaction-using-Graph-Neural-Network/blob/main/Images/resultsp_plot.png)



* Based on the test metrics, we see that SAGE performs the best on drug-drug interaction, closely followed by DGCNN

### What are the remaining portions in this project

* Currently, we have not used any node embeddings initially. Exploring Deepwalk and Node2Vec for node embeddings and comparing results is yet to be done.

### Top few learning
* Given the different techniques and implementations of Link Prediction - GraphSAGE, GCN , DGCNN, GIN – Putting them all together into one framework so that we don’t have to re-code train, test and evaluation based on different formats of implementation.
* Fascinating to model and learn the inner workings of drug-drug interactions via Graph Neural Networks.
* Key choice of evaluation metrics, overcoming hurdles of compute resource shortage.

### References
* Link Prediction Based on Graph Neural Network by Muhan Zhang, Yixin Chen
* DGCNN: Disordered Graph Convolutional Neural Network Based on the Gaussian Mixture Model by Bo Wu, Yang Liu, Bo Lang, Lei Huang
* Semi-Supervised Classification with Graph Convolutional Networks by Semi-Supervised Classification with Graph Convolutional Networks

##### Part of Network Analysis and Mining course 2022 @PES University
