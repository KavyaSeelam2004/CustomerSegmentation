📌 Customer Segmentation using RFM & KMeans
🔹 About Machine Learning

Machine Learning (ML) is a subset of Artificial Intelligence (AI) that allows systems to learn and improve from experience without being explicitly programmed.

Supervised Learning: Model learns from labeled data (e.g., predicting house prices).

Unsupervised Learning: Model finds hidden patterns in unlabeled data (e.g., customer segmentation).

Reinforcement Learning: Model learns by interacting with an environment and receiving feedback.

In this project, we focus on Unsupervised Learning with KMeans Clustering to group customers based on their purchasing behavior.

🔹 Project Overview

The goal of this project is to segment customers of an online retail store into distinct groups using RFM analysis (Recency, Frequency, Monetary). This helps businesses understand customer behavior and design targeted marketing strategies.

Recency (R): How recently a customer purchased.

Frequency (F): How often a customer purchased.

Monetary (M): How much a customer spent.

We apply KMeans clustering on scaled RFM features to identify meaningful customer segments.

🔹 Workflow

Data Preprocessing

Removed missing CustomerIDs

Dropped negative Quantity and UnitPrice values

Created TotalPrice = Quantity × UnitPrice

Feature Engineering (RFM Model)

Calculated Recency, Frequency, and Monetary values per customer

Built an RFM DataFrame

Data Scaling

Standardized RFM features using StandardScaler

Modeling with KMeans

Used the Elbow Method to find optimal clusters

Applied KMeans(n_clusters=4) to group customers

Results & Visualization

Cluster profiling with mean RFM values

Plotted cluster distribution using Seaborn pairplots

🔹 Key Insights

Different groups of customers show varied spending behavior.

Businesses can use these clusters for personalized marketing, loyalty programs, or targeted promotions.

🔹 Tech Stack

Python

Pandas, NumPy – Data preprocessing

Scikit-learn – Scaling & clustering

Matplotlib, Seaborn – Visualization
