# Facebook-Friendship-Prediction
### Facebook Friend Recommendation Using Graph Mining

![Rice31-hairball2-768x709](https://user-images.githubusercontent.com/91129320/148690128-0abd9e71-6735-4c1e-82c0-c8b52ada8dc9.png)


# Real-world / Business

### Problem Statment

Given a directed graph of Instagram's data, we have to predict missing or possible futures links between users and by links here we mean frienship or following relationship.

*****************************

### objectives and constraints

**Objectives:**


Probaility of a possible link is useful in order to recommand and focus on a links with high probability.


*****************************

**Constraints:**

No low-latency requirment is needed [Update on this kind of data may happen once per day or every two days].

*****************************

### ML Problem Formulation


We can map this problem into binary classification problem as follow:

Label the presence of link between two vertex in graph to 1 and 0 otherwise so we need to featurize data in order to help us solving this problem.

*****************************

### Performance metrics

The fact that we recommand the useful link is important [**Precision**] so we don't need to recommend any not realtive links link recommending someone with no relative information or from another country, also if there is connection in real word we should recommand it successfully [**Recall**] here is important as well, so we need two performance metrices:


*   Precision , Recall hence F1-Score is important.
*   Confusion Matrix

*****************************

### Data Overview

Data has taken from Facebook recruting challange took place on Kagle https://www.kaggle.com/c/FacebookRecruiting.
This data is Instagram based data as the links between edge is directed (one side edge), this data could not be from facebook because of the graph type, but for the sake of confidentiality and privacy of theire users Facebook would not publish any information about the data regarding this issue.

data contain two columns source and destination node for each row and it's as follow:
    
    - Data columns (total 2 columns):  
    - source_node         int64  
    - destination_node    int64 

*****************************
