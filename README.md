# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import dataset and print head,info of the dataset
2. check for null values
3. Import kmeans and fit it to the dataset
4. Plot the graph using elbow method
5. Print the predicted array
6. Plot the customer segments

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: IBRAHIM FEDAH S
RegisterNumber: 212223240056


import pandas as pd

import matplotlib.pyplot as plt

data=pd.read_csv("/content/Mall_Customers (1).csv")

data.head()

data.info()

data.isnull().sum()

from sklearn.cluster import KMeans

wcss=[]

for i in range(1,11):

kmeans=KMeans(n_clusters=i,init="k-means++")

kmeans.fit(data.iloc[:,3:])

wcss.append(kmeans.inertia_)

plt.plot(range(1,11),wcss)

plt.xlabel("No_of_Clusters")

plt.ylabel("wcss")

plt.title("Elbow Method")

km=KMeans(n_clusters=5)

km.fit(data.iloc[:,3:])

y_pred=km.predict(data.iloc[:,3:])

y_pred

data["cluster"]=y_pred

df0=data[data["cluster"]==0]

df1=data[data["cluster"]==1]

df2=data[data["cluster"]==2]

df3=data[data["cluster"]==3]

df4=data[data["cluster"]==4]

plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")

plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="black",label="cluster1")

plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="blue",label="cluster2")

plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="cluster3")

plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label="cluster4")

plt.legend()

plt.title("Customer Segment")
*/
```

## Output:

## 1.DATA.HEAD():

![image](https://github.com/user-attachments/assets/a2f304d2-9b43-456b-af44-12946271f632)

## 2.DATA.INF0():

![image](https://github.com/user-attachments/assets/97d06643-735c-4970-9226-69e7e3ec07af)


## 3.DATA.ISNULL().SUM():

![image](https://github.com/user-attachments/assets/413a83f3-cd57-4002-b992-e2a7bd25bad0)


## 4.PLOT USING ELBOW METHOD:

![image](https://github.com/user-attachments/assets/f49d838c-e63b-4f7e-b605-cc64dafe5da6)

## 5.K-MEANS CLUSTERING:

![image](https://github.com/user-attachments/assets/d23f1268-f4b2-4f1a-a810-6e3c8a71dc9c)


## 6.Y_PRED ARRAY:

![image](https://github.com/user-attachments/assets/7ffc78af-df39-4c64-94ec-4d1122f8cf80)


## 7.CUSTOMER SEGMENT:

![image](https://github.com/user-attachments/assets/5e2d1532-4d53-4543-b359-968dbe8d6c04)



## Result:

Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.







