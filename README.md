# Google-Landmark-Recognition

<b>Aim of the Project :</b> 
Did you ever go through your vacation photos and ask yourself: What is the name of this temple I visited in China? Who created this monument I saw in France? Landmark recognition can help! This technology can predict landmark labels directly from image pixels, to help people better understand and organize their photo collections.

Today, a great obstacle to landmark recognition research is the lack of large annotated datasets. Here we present the largest worldwide dataset to date, to foster progress in this problem. This Project challenges to build models that recognize the correct landmark (if any) in a dataset of challenging test images.

<b>Description :</b> 
Submissions are evaluated using Global Average Precision (GAP) at k, where k=1. This metric is also known as micro Average Precision (microAP).It works as follows:
For each query image, you will predict one landmark label and a corresponding confidence score. The evaluation treats each prediction as an individual data point in a long list of predictions (sorted in descending order by confidence scores), and computes the Average Precision based on this list.

If a submission has N predictions (label/confidence pairs) sorted in descending order by their confidence scores, then the Global Average Precision is computed as:

GAP = \frac{1}{M}\sum_{i=1}^N P(i) rel(i)

where:

N is the total number of predictions returned by the system, across all queries
M is the total number of queries with at least one landmark from the training set visible in it (note that some queries may not depict landmarks)
P(i) is the precision at rank i
rel(i) denotes the relevance of prediciton i: it’s 1 if the i-th prediction is correct, and 0 otherwise



