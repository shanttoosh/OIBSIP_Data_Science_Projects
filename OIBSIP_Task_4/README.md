# Customer Segmentation Machine Learning Model

As part of my internship at Oasis Infobyte, I successfully completed my fourth task: Customer Segmentation Machine Learning Model using k means.This project focuses on customer segmentation using the K-Means clustering algorithm to identify distinct customer groups based on their purchasing behavior. By analyzing key metrics such as Recency, Frequency, and Monetary value (RFM), we aim to provide actionable insights that can help businesses tailor their marketing strategies and enhance customer engagement.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Loading](#data-loading)
3. [Data Cleaning](#data-cleaning)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Feature Engineering](#feature-engineering)
6. [Scaling](#scaling)
7. [Model Building](#model-building)
8. [Model Evaluation](#model-evaluation)
9. [Cluster Analysis](#cluster-analysis)
10. [Conclusion](#conclusion)

## Project Overview
Customer segmentation is a crucial task for businesses aiming to tailor their marketing strategies to different customer groups. This project utilizes the K-Means clustering algorithm to segment customers based on their purchasing behavior. By identifying distinct segments, businesses can better understand their customer base and apply targeted marketing strategies to improve customer satisfaction and increase sales.

The project is structured as follows:
- **Data Loading**: Importing and understanding the dataset.
- **Data Cleaning**: Preparing the data for analysis by handling missing values, duplicates, and outliers.
- **Exploratory Data Analysis (EDA)**: Gaining insights into customer behavior through data visualization and descriptive statistics.
- **Feature Engineering**: Creating and selecting features that are most relevant for customer segmentation.
- **Scaling**: Standardizing the data to ensure that all features contribute equally to the clustering process.
- **Model Building**: Applying the K-Means algorithm to create customer segments.
- **Model Evaluation**: Assessing the quality of the segments using evaluation metrics.
- **Cluster Analysis**: Interpreting the characteristics of each customer segment to derive actionable insights.

## Data Loading
The dataset used in this project is loaded from a CSV file. The initial exploration includes examining the first few rows of the dataset to understand the structure, checking for any inconsistencies, and identifying key variables.

**Steps Involved:**
- Use `pandas` to load the dataset.
- Display the first few rows using `head()` to get a quick overview.
- Check the data types of each column using `dtypes` to ensure they are appropriate for analysis.
- Identify the target variables (e.g., customer spending, frequency of purchases) and features that will be used in clustering.

## Data Cleaning
Data cleaning is a critical step in any data analysis project. In this project, the data cleaning process involves handling missing values, removing duplicates, and dealing with outliers. These steps ensure the integrity of the data, which is essential for accurate clustering.

**Steps Involved:**
- **Handling Missing Values**: Use `isnull().sum()` to identify missing values. Depending on the extent of missing data, either impute missing values using techniques such as mean/mode imputation or drop rows/columns with excessive missing data.
- **Removing Duplicates**: Check for duplicate rows using `duplicated()` and remove them to avoid skewing the clustering results.
- **Outlier Detection**: Use visualization techniques such as box plots to identify outliers. Depending on the context, outliers may be removed or treated differently (e.g., capping).

## Exploratory Data Analysis (EDA)
Exploratory Data Analysis (EDA) helps in understanding the underlying patterns in the data. In this project, EDA focuses on analyzing customer behavior in terms of recency (how recently they made a purchase), frequency (how often they purchase), and monetary value (how much they spend). 

**Steps Involved:**
- **Descriptive Statistics**: Generate summary statistics (mean, median, standard deviation) for key variables to understand the central tendency and dispersion.
- **Visualizations**: Use histograms, box plots, and scatter plots to visualize the distribution of variables and identify any patterns or anomalies.
- **Correlation Analysis**: Examine correlations between variables to understand relationships and dependencies that might affect clustering.

## Feature Engineering
Feature engineering involves creating new features or transforming existing ones to improve the performance of the clustering algorithm. In this project, features such as Recency, Frequency, and Monetary value (RFM) are crucial for segmentation.

**Steps Involved:**
- **Creating RFM Features**: Calculate Recency (days since last purchase), Frequency (total number of purchases), and Monetary value (total amount spent) for each customer.
- **Log Transformations**: Apply log transformations to skewed data to normalize the distribution, which can improve the clustering results.
- **Dimensionality Reduction**: Consider using techniques such as PCA (Principal Component Analysis) if the dataset has a large number of features, to reduce dimensionality and focus on the most significant variables.

## Scaling
Scaling is an important preprocessing step in clustering algorithms like K-Means, which are sensitive to the scale of the input data. By standardizing the data, we ensure that all features contribute equally to the clustering process.

**Steps Involved:**
- **Standardization**: Use `StandardScaler` from `sklearn` to standardize the features so that they have a mean of 0 and a standard deviation of 1.
- **Verification**: After scaling, verify the transformed data by checking summary statistics to ensure that the scaling has been applied correctly.

## Model Building
The core of this project is building the K-Means clustering model. K-Means is an unsupervised learning algorithm that partitions customers into K distinct clusters based on their RFM features.

**Steps Involved:**
- **Choosing the Number of Clusters (K)**: Use the Elbow Method or Silhouette Score to determine the optimal number of clusters.
- **Applying K-Means**: Use `KMeans` from `sklearn` to fit the model to the standardized data.
- **Cluster Assignment**: Each customer is assigned to a cluster, which is stored in a new column in the dataset.

## Model Evaluation
Evaluating the clustering model is crucial to ensure that the clusters are meaningful and well-separated. The quality of the clusters is assessed using metrics like the Silhouette Score.

**Steps Involved:**
- **Silhouette Score**: Calculate the Silhouette Score to evaluate how well the clusters are separated. A higher score indicates better-defined clusters.
- **Cluster Visualization**: Plot the clusters using 2D or 3D scatter plots to visually assess their separation.

## Cluster Analysis
After the clusters are formed, it's important to analyze them to understand the characteristics of each customer segment. This analysis helps in deriving actionable insights that can inform marketing strategies.

**Steps Involved:**
- **Cluster Profiles**: Analyze the mean RFM values for each cluster to understand the typical customer in each segment.
- **Visualization**: Create bar charts, box plots, or heatmaps to visualize the differences between clusters.
- **Business Insights**: Based on the analysis, provide recommendations on how to target each customer segment (e.g., high spenders vs. frequent buyers).

## Conclusion
This project successfully segments customers into distinct groups based on their purchasing behavior. The insights gained from this segmentation can be used to tailor marketing strategies, improve customer satisfaction, and ultimately drive sales growth. The approach used in this project can be applied to other customer datasets to achieve similar objectives.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Connect with Me

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/shanttoosh-v-470484289/) and follow my journey in data analytics and visualization!


