# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Choose the number of clusters (K).

2. Randomly initialize K centroids.

3. Assign each data point to the nearest centroid.

4. Recalculate the centroids.

5. Repeat steps 3 and 4 until centroids do not change

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: Shankar S B
RegisterNumber: 212225230260

# Simple K-Means Clustering Program for Customer Segmentation

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

data = pd.read_csv("Mall_Customer.csv")

X = data.iloc[:, [3, 4]].values

kmeans = KMeans(n_clusters=5, random_state=0)

y_kmeans = kmeans.fit_predict(X)

plt.scatter(X[:, 0], X[:, 1], c=y_kmeans, s=50)

# Plot centroids
plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200,
            marker='X')

# Labels
plt.xlabel("Annual Income")
plt.ylabel("Spending Score")
plt.title("Customer Segmentation using K-Means")

plt.show()
*/
```

## Output:
<img width="786" height="576" alt="Screenshot 2026-05-15 143810" src="https://github.com/user-attachments/assets/7d0198a6-1d52-4d66-a210-88720fe99736" />



## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
