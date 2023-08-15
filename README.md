# Industrial-Copper-Modeling
# Problem Statement
The copper industry faces challenges in accurately predicting sales and pricing due to skewed and noisy data. Manual predictions may not yield optimal results, leading to time wastage. To mitigate this, a machine learning regression model is proposed. This model will employ advanced techniques like data normalization, feature scaling, and outlier detection to enhance accuracy and address data issues.

Another challenge is lead classification, where predicting potential customers is vital. A lead classification model is required, utilizing the STATUS variable (WON for Success and LOST for Failure). Non-WON and LOST data points should be removed.

The proposed solution involves these steps:

Explore dataset skewness and outliers.
Transform and preprocess data for analysis.
Develop an ML regression model for predicting 'Selling_Price'.
Create an ML classification model to predict Status (WON/LOST).
Build a Streamlit page for easy input and output of column values for Selling_Price or Status predictions.

# Aim
The aim of this project is to enhance the efficiency and accuracy of sales and lead management in the copper industry by leveraging machine learning techniques. Specifically, the project aims to develop a comprehensive solution that addresses challenges related to skewed, noisy data in sales and pricing, and the identification of potential customer leads. By applying advanced methods such as data normalization, feature scaling, and outlier detection, the project seeks to build robust machine learning regression and classification models.

The project's primary objectives include:

## Data Analysis and Preparation: 
Explore the provided dataset to identify skewness and outliers, and undertake necessary data cleaning and preprocessing steps to ensure the data's quality and reliability.

## Regression Model Development: 
Create a machine learning regression model capable of predicting the continuous variable 'Selling_Price' with high accuracy. This model will serve as a valuable tool for optimizing pricing decisions.

## Classification Model Development: 
Develop a lead classification model utilizing the 'STATUS' variable, classifying leads as 'WON' or 'LOST' based on their likelihood of becoming a customer. Data points other than 'WON' and 'LOST' statuses will be excluded for accurate lead evaluation.

## Streamlit Application: 
Design and implement a user-friendly Streamlit application that allows users to input relevant data for predicting selling prices or lead statuses. The application's interface will facilitate quick and informed decision-making by providing real-time predictions.

# Requirements 
* NumPy
* Python
* Pandas
* Scikit-learn
* Streamlit
* Matplotlib
* Seaborn

# Methods
* Importing the necessary modules
* Detecting skewness and outliers in the given data set
* Preprocessing the data set
* Training the Model
* Evaluating the Model

# Workflow
* Data Understanding: Identify the types of variables (continuous, categorical) and their distributions. Some rubbish values are present in ‘Material_Reference’ which starts with ‘00000’ value

* Data Preprocessing: ● Handle missing values, outliers, and skewness in the dataset. ● Apply appropriate data transformations, such as log transformation, boxcox transformation, or other techniques, to handle skewness in continuous variables. ● Encode categorical variables using suitable techniques, such as one-hot encoding, label encoding, or ordinal encoding, based on their nature and relationship with the target variable

* EDA: Try visualizing outliers and skewness using Seaborn’s boxplot, distplot, violinplot

* Feature Engineering: Engineer new features if applicable, such as aggregating or transforming existing features to create more informative representations of the data. And drop highly correlated columns

* Model Building and Evaluation: ● Split the dataset into training and testing/validation sets. ● Train and evaluate different classification models, such as ExtraTreesClassifier, XGBClassifier, or Logistic Regression, using appropriate evaluation metrics such as accuracy, precision, recall, F1 score, and AUC curve. ● Optimize model hyperparameters using techniques such as cross-validation and grid search to find the best-performing model

* Model GUI: Using streamlit module, create interactive page with task input( Regression or Classification) and create an input field where you can enter each column value except ‘Selling_Price’ for regression model and except ‘Status’ for classification model

