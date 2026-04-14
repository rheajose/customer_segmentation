# Customer Segmentation — K-Means Clustering

## Overview
An unsupervised machine learning model that segments retail store
customers into distinct groups based on their annual income and
spending behaviour, using the Mall Customer dataset from Kaggle.

## Dataset
Source: https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python
Samples: 200 customers
Features used: Age, Annual Income, Spending Score, Gender

## Approach
1. Exploratory Data Analysis — distributions, gender split, scatter plots
2. Feature selection — Annual Income and Spending Score as primary features
3. StandardScaler normalisation
4. Elbow method to determine optimal K
5. KMeans clustering with K=5
6. Business interpretation of each customer segment

## Results — 5 Customer Segments Identified
| Cluster | Label | Avg Income | Avg Spending |
|---------|-------|------------|--------------|
| 0 | Prime targets | High | High |
| 1 | At-risk | Low | Low |
| 2 | Savers | High | Low |
| 3 | Impulsive buyers | Low | High |
| 4 | Average customers | Medium | Medium |

## Project Structure
├── customer_segmentation.ipynb   # Full notebook with outputs
├── elbow_curve.png               # Optimal K selection chart
├── customer_clusters.png         # Final cluster visualisation
├── pairplot_clusters.png         # Feature relationships by cluster
├── income_vs_spending.png        # EDA scatter plot
├── feature_distributions.png     # Feature distribution charts
├── gender_distribution.png       # Gender breakdown
├── requirements.txt              # Python dependencies
└── README.md                     # This file

## How to Run
1. git clone https://github.com/rheajose/customer_segmentation.git
2. pip install -r requirements.txt
3. Download Mall_Customers.csv from Kaggle and place in project folder
4. jupyter notebook customer_segmentation.ipynb

## Tools & Libraries
- Python 3.9+
- pandas, numpy
- scikit-learn (KMeans, StandardScaler)
- matplotlib, seaborn
- Jupyter Notebook

## Skills Demonstrated
- Unsupervised machine learning (K-Means clustering)
- Elbow method for hyperparameter tuning
- Customer segmentation and business interpretation
- Data visualisation and storytelling
