# Player-Segmentation-Using K_Means 
This repository represent an unsupervised machine learning approach to segment FIFA players using the K-means clustering algorithm. The goal is to group players with similar attributes to enable deeper analysis and better understanding of player profiles.

## 📌 Project Overview
This project applies unsupervised machine learning to group professional football players based on attributes such as skill level, market value, wages, and age. Using a custom implementation of the KMeans clustering algorithm, we aim to identify patterns and similarities between players without any prior labels. This approach can help scouts, analysts, and managers explore player categories for decision-making.

## 📊 Dataset
The dataset is sourced from the FIFA player database and includes a wide range of player features. For clustering purposes, we selected the following numerical attributes:

**overall** – Player's overall rating

**potential** – Predicted maximum rating

**value_eur** – Market value in Euros

**wage_eur** – Weekly wage

**age** – Player's age

## ⚙ Clustering Process
Instead of using built-in libraries, we implemented KMeans from scratch to understand the algorithm in depth.    
steps:

🎲 **Random Initialization:**
Centroids are initialized by randomly sampling values from the dataset, ensuring realistic starting points.

🎯 **Assignment Step:**
Each player is assigned to the nearest centroid based on Euclidean distance.

🔁 **Update Step:**
New centroids are calculated using the geometric mean of points in each cluster (more stable for normalized data).

**📉 Iteration & Visualization:**
The process repeats until centroids stabilize or max iterations are reached. We used PCA to reduce the feature space to 2D and visualize the clustering process dynamically.

## 📈 Key Observations
✅ Players with high overall and potential ratings tend to cluster together, typically reflecting elite players.

✅ Low-value, low-wage players form distinct groups, likely representing younger or less experienced players.

✅ Market value and wages are highly correlated and often dominate the clustering behavior.

## 📁 Dataset
The dataset used is publicly available on Kaggle:

https://www.kaggle.com/datasets/stefanoleone992/fifa-23-complete-player-dataset

## 🤝 Contributions
Contributions to this project are welcome. If you find any issues, have suggestions for improvements, or want to contribute new features, please feel free to submit a pull request.

## 📄 License
This project is licensed under the MIT License. You are free to use, modify, and distribute the code in this repository, subject to the terms and conditions of the license.

## 👩‍💻 Author & Contact       
📌 Project by: Nazanin Mahmoudy, 2025                    
📧 Email: Nazaninmahmoudy@gmail.com                     
🔗 GitHub: https://github.com/Nazaninmahmoudi                      
🔗 Kaggle: https://www.kaggle.com/nazaninmahmoudy                             
