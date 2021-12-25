# Social Network Graph Link Prediction - Facebook Challenge

**Problem Statement**

Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph).

**Data Overview**

Taken data from facebook's recruting challenge on [Kaggle](https://www.kaggle.com/c/FacebookRecruiting).

Data contains two columns source and destination eac edge in graph.

- Data Columns (total 2 columns):  
- source_node         int64  
- destination_node    int64  

**Mapping the problem into supervised learning problem**

Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link.

**Business Objectives and Constraints**
- No low-latency requirement
- Probability of prediction is useful to recommend ighest probability links

**Performance metric for supervised learning**
- Both precision and recall is important so F1 score is good choice
- Confusion matrix

*Posing a Problem as a Classification Problem*
[Click Here]() To Check Exploratory Data Analysis - 1_FB_EDA_
[Click Here]() To Check Work on The Features (Extraction) - 2_FB_Featurization_
[Click Here]() To Check Work on Models (ML) - 3_FB_Models_

### Machine Learning Models

| Models | Train F1 Score | TestF1 Score |
|--------|----------------|--------------|
| Random Forest | 0.96 | 0.92 |
| XG Boost | 1.0 | 0.92 |

