🛍️ Customer Segmentation Using Unsupervised Learning

🎯 Objective:

Cluster customers based on their spending habits and propose targeted marketing strategies for each segment.

📊 Dataset:



Mall Customers Dataset – contains demographic and spending information for mall customers:

Column	Description
CustomerID	Unique ID for each customer
Gender	Male/Female
Age	Age of the customer
Annual Income (k$)	Annual income in thousands of dollars
Spending Score (1-100)	Score assigned by the mall based on customer behavior


📝 Project Steps:

Step 1: Import Libraries

Python libraries used:

pandas, numpy → data handling

matplotlib, seaborn → visualization

sklearn → preprocessing, K-Means, PCA, t-SNE

Step 2: Load Dataset

Load CSV using latin1 encoding to avoid errors.

Inspect the dataset with .head(), .info(), .describe().

Step 3: Exploratory Data Analysis (EDA)

Visualize relationships between features using pairplots.

Identify correlations with a heatmap.

Observe customer distribution across age, income, and spending score.

Step 4: Data Preprocessing

Select key features for clustering: Annual Income and Spending Score.

Standardize features using StandardScaler for uniform scaling.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b77ed0d8-bc1f-45ab-a39e-10ddee31c79d" />


Step 5: Determine Optimal Number of Clusters

Use Elbow Method with K-Means inertia to find the ideal number of clusters (commonly 5).

Plot number of clusters vs inertia to visually identify the elbow point.

Step 6: Apply K-Means Clustering

Fit K-Means with the chosen number of clusters.

Assign cluster labels to each customer for segmentation.

Step 7: Visualize Clusters

PCA Visualization: Reduce features to 2 components and plot clusters.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8a37eabe-de2a-4b0a-8c59-4c4d1cbe6697" />


t-SNE Visualization (Optional): Capture complex relationships in 2D for better visualization.

Step 8: Analyze Cluster Characteristics

Calculate mean Age, Annual Income, and Spending Score for each cluster.

Identify spending patterns and demographic trends for each group.

Step 9: Propose Marketing Strategies

High spending customers (Spending Score > 60) → premium products, loyalty programs.

Medium spending customers (Spending Score 40-60) → cross-sell, upsell opportunities.

Low spending customers (Spending Score < 40) → discounts, promotions, engagement campaigns.
