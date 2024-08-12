# House Price Prediction

As part of my internship at Oasis Infobyte, I successfully completed my third task: House Price Prediction. House prices based on various features using Linear Regression and Gradient Boosting Regressor. The dataset contains various attributes related to houses, including area, number of bedrooms, number of bathrooms, and more.

## 📋 Table of Contents

1. [📂 Dataset](#dataset)
2. [🔧 Data Preprocessing](#data-preprocessing)
   - [Encoding Categorical Variables](#encoding-categorical-variables)
   - [Feature Engineering](#feature-engineering)
   - [Scaling Numerical Features](#scaling-numerical-features)
   - [Handling Outliers](#handling-outliers)
   - [Handling Missing and Duplicate Values](#handling-missing-and-duplicate-values)
3. [📊 Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
   - [Boxplot for Outlier Detection](#boxplot-for-outlier-detection)
   - [Histogram for Distribution of House Prices](#histogram-for-distribution-of-house-prices)
   - [Scatter Plot with Linear Regression](#scatter-plot-with-linear-regression)
   - [FacetGrid for Price Distribution by Number of Bedrooms](#facetgrid-for-price-distribution-by-number-of-bedrooms)
   - [Correlation Matrix and PairPlot](#correlation-matrix-and-pairplot)
4. [🛠️ Model Training](#model-training)
   - [Linear Regression](#linear-regression)
   - [Gradient Boosting Regressor](#gradient-boosting-regressor)
5. [📈 Model Evaluation](#model-evaluation)
6. [📉 Visualization](#visualization)
7. [🔧 Requirements](#requirements)
8. [⚙️ Usage](#usage)
9. [📝 License](#license)
10. [🤝 Connect with Me](#connect-with-me)
11. [📚 Resources](#resources)

## 1. 📂 Dataset

The dataset used for this project is `Housing.csv` and includes the following columns:

- `price`: The price of the house
- `area`: The area of the house in square feet
- `bedrooms`: The number of bedrooms
- `bathrooms`: The number of bathrooms
- `stories`: The number of stories
- `mainroad`: Whether the house is on the main road (yes/no)
- `guestroom`: Whether there is a guestroom (yes/no)
- `basement`: Whether there is a basement (yes/no)
- `hotwaterheating`: Whether there is hot water heating (yes/no)
- `airconditioning`: Whether there is air conditioning (yes/no)
- `parking`: The number of parking spaces
- `prefarea`: Whether the house is in a preferred area (yes/no)
- `furnishingstatus`: The furnishing status (furnished/semi-furnished/unfurnished)

## 2. 🔧 Data Preprocessing

### Encoding Categorical Variables

Categorical variables are encoded using `LabelEncoder`.

### Feature Engineering

- `price_per_area`: Price divided by area
- `bed_bath_interaction`: Product of the number of bedrooms and bathrooms
- `log_price`: Logarithm of the price

### Scaling Numerical Features

Features are standardized using `StandardScaler`.

### Handling Outliers

Outliers are capped based on the Interquartile Range (IQR).

### Handling Missing and Duplicate Values

- **Missing Values:** Identifying null values
- **Duplicate Values:** Identifying duplicate values

## 3. 📊 Exploratory Data Analysis (EDA)

### Boxplot for Outlier Detection

Boxplots are used to visualize outliers in various features.

### Histogram for Distribution of House Prices

A histogram is created to visualize the distribution of house prices.

### Scatter Plot with Linear Regression

A scatter plot with a regression line shows the relationship between area and price.

### FacetGrid for Price Distribution by Number of Bedrooms

Histograms for price distribution are shown for different numbers of bedrooms.

### Correlation Matrix and PairPlot

A heatmap of the correlation matrix and a pair plot are used to analyze feature relationships with the target variable (`price`).

## 4. 🛠️ Model Training

### Linear Regression

- Coefficients and intercept are obtained.
- Model evaluation metrics include Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²).

## 5. 📈 Model Evaluation

- **Linear Regression:**
  - Mean Squared Error (MSE): 186,712,020,979.23
  - Root Mean Squared Error (RMSE): 432,101.86
  - R-squared (R²): 0.9538

- **Gradient Boosting Regressor:**
  - Mean Squared Error (MSE): 235,255,200.21
  - Root Mean Squared Error (RMSE): 15,338.03
  - R-squared (R²): 0.9999

## 6. 📉 Visualization

- **Actual vs. Predicted Values:**
  A scatter plot visualizes the comparison between actual and predicted house prices.

## 7. 🔧 Requirements

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `google.colab` (for file upload)

## 8. ⚙️ Usage

1. Upload the dataset using `files.upload()`.
2. Run the data preprocessing, EDA, and model training code.
3. Evaluate the models and visualize the results.

## 9. 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 10. 🤝 Connect with Me

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/shanttoosh-v-470484289/) and follow my journey in data analytics and visualization!

## 11. 📚 Resources

- **Google:** [Google Colab](https://colab.research.google.com/)
- **Data Source:** [Kaggle: Housing Price Prediction](https://www.kaggle.com/code/ashydv/housing-price-prediction-linear-regression)
