
# 🏠 Airbnb NYC 2019 Data Cleaning Project

As part of my internship at Oasis Infobyte, I successfully completed my second task: Data Cleaning. This project involves the preprocessing of the Airbnb NYC 2019 dataset. The primary goal is to clean the data, handle missing values, identify and treat outliers, and prepare the dataset for further analysis or modeling.

---

## 📚 Table of Contents

1. [Introduction](#-introduction)
2. [Dataset](#-dataset)
3. [Dataset Features](#-dataset-features)
4. [Project Structure](#-project-structure)
5. [Data Cleaning Process](#-data-cleaning-process)
   - [Handling Missing Values](#-handling-missing-values)
   - [Handling Duplicates](#-handling-duplicates)
   - [Cleaning String Columns](#-cleaning-string-columns)
   - [Standardizing Numerical Values](#-standardizing-numerical-values)
   - [Handling Outliers](#-handling-outliers)
6. [Running the Analysis](#-running-the-analysis)
7. [Link to Repository](#-link-to-repository)
8. [Connect with Me](#-connect-with-me)
9. [Resources](#-resources)

---

## 1. 🏠 Introduction

As part of my internship at Oasis Infobyte, I successfully completed my second task: Data Cleaning. This project involves the preprocessing of the Airbnb NYC 2019 dataset. The primary goal is to clean the data, handle missing values, identify and treat outliers, and prepare the dataset for further analysis or modeling.

---

## 2. 📊 Dataset

The dataset used in this project is `AB_NYC_2019.csv`, which contains information about Airbnb listings in New York City as of 2019.

---

## 3. 📑 Dataset Features

The dataset consists of 48,895 entries and 16 columns:

- `id`: Unique identifier for each listing
- `name`: Name of the listing
- `host_id`: Unique identifier for the host
- `host_name`: Name of the host
- `neighbourhood_group`: Borough where the listing is located
- `neighbourhood`: Specific neighborhood within the borough
- `latitude`: Latitude of the listing
- `longitude`: Longitude of the listing
- `room_type`: Type of room being listed
- `price`: Price per night
- `minimum_nights`: Minimum number of nights required to book
- `number_of_reviews`: Total number of reviews received
- `last_review`: Date of the last review
- `reviews_per_month`: Average number of reviews per month
- `calculated_host_listings_count`: Number of listings the host has
- `availability_365`: Number of days the listing is available in a year

---

## 4. 🗂 Project Structure

- `data`: Directory containing the dataset file `AB_NYC_2019.csv`
- `notebooks`: Directory containing Jupyter notebooks for data analysis
- `README.md`: Project documentation

---

## 5. 🧹 Data Cleaning Process

The following steps were performed to clean and preprocess the data:

### 📉 Handling Missing Values

- Identified columns with missing values: `name`, `host_name`, `last_review`, and `reviews_per_month`.
- Dropped rows with missing values to simplify analysis.

### 🔄 Handling Duplicates

- Checked for duplicate entries and confirmed that there were no duplicates in the dataset.

### 🧽 Cleaning String Columns

- Removed special characters and numeric values from non-numeric columns such as `name`, `host_name`, and `neighbourhood`.

### 🔢 Standardizing Numerical Values

- Scaled numerical features such as `availability_365`, `calculated_host_listings_count`, `reviews_per_month`, `number_of_reviews`, `minimum_nights`, and `price` using `StandardScaler`.

### 📏 Handling Outliers

- Detected outliers using the Interquartile Range (IQR) method.
- Replaced outliers with the median values of the respective columns to maintain data consistency.

---

## 6. 🚀 Running the Analysis

To run the analysis, clone the repository:

```bash
git clone <repository-url>

## 7. 📌 Link to Repository

[Repository Link](https://github.com/shanttoosh/OIBSIP_Data_Science_Projects/tree/main/OIBSIP_Task_1)

---

## 8. 🤝 Connect with Me

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/shanttoosh-v-470484289/) and follow my journey in data analytics and visualization!

---

## 9. 📚 Resources

- **Google:** [Google Colab](https://colab.research.google.com/)
- **Data Source:** [Kaggle: New York City Airbnb Open Data](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)





   
