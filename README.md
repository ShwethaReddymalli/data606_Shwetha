
# LUNG CANCER PREDICTION USING MACHINE LEARNING MODELS

## Name: Shwetha Reddy Reddymalli
<br />

Here is the dataset download link: https://www.kaggle.com/datasets/rishidamarla/cancer-patients-data?select=cancer+patient+data+sets.xlsx

Youtube video link: https://www.youtube.com/watch?v=6Jo3xUdL0-c

## INTRODUCTION

<p align='justify'>Lung Cancer is categorized as the third most common cancer in the United States. The statistics state that more people die from Lung Cancer than any other type of cancer. Most people with lung cancer do not have any symptoms until it is reached an advanced stage. Mostly frequent coughing and chest pain are considered the symptoms of lung cancer. According to an estimation, 2,36,740 people will be diagnosed in the USA in 2022. The research also states that one in 16 people will be diagnosed with lung cancer in their lifetime. Lung Cancer is usually treated in several ways, based on its spread and type. People with small cell lung cancer are usually treated with radiation therapy and chemotherapy. Sometimes doctors cut out the cancer tissue through surgery and sometimes processes targeted therapy.
<br />

**Lung Cancer-By the numbers** 
<br />
<br />
<img src="https://images.ctfassets.net/yixw23k2v6vo/1OP4r4gfD87wjbCf4KjLOr/a4a306da0ed8380f3bdba2bf6979a578/LUNG_INFO_stats.png?fit=thumb&w=1648&h=928" width="550"/>
<br />

## Dataset Insights

<p align='justify'>The dataset is considered from Kaggle. This contains a total of 1000 rows and 25 columns. The data type of each of these columns is an integer, except for patient_id and level which are strings. The dataset is categorized into two different levels based on the records of the patients.
<br />

[Dataset Link](https://www.kaggle.com/datasets/rishidamarla/cancer-patients-data?select=cancer+patient+data+sets.xlsx)
<br />

<p align='justify'>TThis dataset contains a total of 1000 rows and 25 columns. The data type of each of these columns is an integer, except for patient_id and level which are strings. The dataset will be categorized into three different levels based on the records of the patients. We will be identifying if there are any null values. We will try to split the entire dataset into 75% and 25% as training and test data respectively. After the initial analysis, we will identify a few non-value-adding columns for our analysis, and those columns will be dropped before we start our analysis. To understand the significance of each column we will be applying Pearson Correlation to our data and a heatmap will be used to understand how few of the features impact our targeted variables. 
<br />

## We will be addressing the below points in our analysis:

1. Identify whether the risk of being affected by lung cancer is higher in Men or Women (gender comparison of data)?

2. Does smoking frequency lead to a higher rate of getting affected?

3. Do older adults affect with cancer experience tendencies of weight loss, shortness of breath, and fatigue?
<br />

## Implementation of Machine Learning Models:

1. Gaussian Naive Bayes

2. Ridge Regression Model

3. Linear Discriminant Analysis

4. Logistic Regression Model

5. K-nearest Neighbor

 ## Results and Conclusion:
<br />
 <p align='justify'>Hypothesis 1 is true. 'High' prone frequency is higher for men than women.<br>
 <p align='justify'>Hypothesis 2 is true. We can observe from the bubbleplot that higher smoking tendency leads to higher chances of Lung diseases.
 <p align='justify'>Hypothesis 3 holds true for Weight loss. People with age >50 have higher chances of Weight loss. However, People with age 30-40 have higher chances of fatigue. It might be because of the reason that the mentioned age group have occupations which deal with mental and physical stress.
<br />


**Machine Learning Models** 
 <p align='justify'>We will be splitting the data into train and test models. I have split the 70 and 30 subsets. One part is used to evaluate and test the data and the other part is used to train the model. I have considered a random state of 102. Once the data is printed for testing and training, we adopted standard scaling using a standard scaler for our analysis, this will help us in removing the mean scaling to unit variance. This will transform our data so that its distribution will have a mean value of 0 and a standard deviation of 1.
<br />

<p align='justify'>The first machine learning model is Gaussian Naive Bayes. Usually, this model is used when they have many independent variables and continuous values, and so is our data. The data set has many independent variables such as different symptoms of lung cancer. When we test the data using this model this resulted in an accuracy of 86%.
 

<p align='justify'>The next model adopted is the Ridge regression model and this model is used for the data with multi-collinear. Our dataset exhibits multicollinearity and hence we have used a standard scaler to normalize the data and implemented the model considering the alpha values as 0.1 and 100. This resulted in an accuracy of 64% and 61% respectively.
<p align='justify'>Linear Discrimination Analysis is used for supervised classification problems and it works great on our data as we have target variables. This model doesn’t work with categorical values hence we used a string indexer to perform the indexing. This model resulted in an accuracy of 95%.

<p align='justify'>The next model considered is the Logistic regression model. This is similar to linear regression but it can be explained as a fast and uncomplicated one. I considered Liblinear as a solver as it suits best our data with a random state of 90. This model resulted in an accuracy of 95%.

<p align='justify'>The final model considered is the K-nearest neighbor model for analyzing the data. This algorithm uses the euclidean distance matrix. I tried to implement cross-validation and grid search to find the best parameters. After considering the best parameter the analysis resulted in an accuracy of 93%

<p align='justify'>The linear discrimination model could produce an accuracy of 96% higher than any other model and can be suggested as the best model for training our data.
<br />

  ## References:

  1. [Lung Cancer Survival Prediction via Machine Learning Regression, Classification, and Statistical Techniques. ](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6634305/#:~:text=Studies%20have%20evaluated%20lung%20cancer%20patient%20survival%20by,%5D%2C%20and%20ensemble%20clustering-based%20approaches%20%5B%206%20%5D.)

2. [Lung cancer prediction using machine learning and advanced imaging techniques. ](https://pubmed.ncbi.nlm.nih.gov/30050768/)

3. https://www.researchgate.net/publication/221649587_Modelling_and_Analysing_Interval_Data
4. https://towardsdatascience.com/data-cleaning-in-python-the-ultimate-guide-2020-c63b88bf0a0d
