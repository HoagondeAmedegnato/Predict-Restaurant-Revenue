# Predict-Restaurant-Revenue
***Its an assignment task to predict the revenue of restaurant***

![image](https://user-images.githubusercontent.com/79173300/152890377-22c9fce0-1886-4873-a9c4-9483d2594b19.png)

____

**Note**: This readme will guide you through the steps I took to complete this project
____
**Table of Contents**
____
I.	***Introduction***

II.	***Data Collection and Data Preprocessing***

III. ***Exploratory Data Analysis and Model Development***: EDA&MODEL.ipynb

IV.	***Findings and Takeaways***
____
I.	***Introduction***

A **fast food restaurant**, also known as a **quick service restaurant (QSR)** within the industry, is a specific type of restaurant that serves fast food cuisine and has minimal table service. The food served in fast food restaurants is typically part of a "meat-sweet diet", offered from a limited menu, cooked in bulk in advance and kept hot, finished and packaged to order, and usually available for take away, though seating may be provided. 

The restaurant is increasing in term of the demand, and as a consequent, is increasing in revenue. Predicting the restaurant revenue for the future is crucial for me as I am determinate and motivated in doing so. This analysis will help me to know more about the future revenue of the restaurant.
____
II.	***Data Collection and Data Preprocessing***

The datasets I use, is from Kaggle website (Data Source: https://www.kaggle.com/sanamps/predict-restaurant-revenue), where two files (train.csv with 43 columns and test.csv with 42 columns) have been provided. The columns names are as follow:
* Id: Restaurant ID
* Open Date: Opening Date of a restaurant
* City: City where restaurant is located
* City Group: Type of the city, Big cities, or Other.
* Type: Type of the restaurant. FC: Food Court, IL: Inline
* P1, P2, P3…. P37: There are three categories of these obfuscated data:
 -- Demographic data are gathered from third party providers with GIS systems. These include population in any given area, age and gender distribution, development scales.
 -- Real estate data mainly relate to the m2 of the location, front facade of the location, car park availability.
 -- Commercial data mainly include the existence of points of interest including schools, banks, other QSR operators.
* Revenue: The revenue column indicates transformed revenue of the restaurant in a given year and is the target of predictive analysis

The train.csv file has 137 rows, and the test.csv file has 100000 rows.

I’ve downloaded the two files CSV from the Kaggle website and save them into my Google Drive, created a Google Colaboratory for the notebook, called EDA&MODEL, in order to analyze, visualize the dataset and to develop the model using the Supervised Machine Learning techniques.
The notebook EDA&MODEL is subdivided into two (2) parts:
* *Exploratory Data Analysis (EDA)*, where I’ve explored the analysis for the overall dataset, proceeded with the visualizations
* *Model Development*, where I’ve calculated the Accuracy Score on the training data and the R-Squared Score on the test data, using the Supervised Machine Learning techniques, such as Logistic Regression, Decision Tree, Support Vector Machines, Random Forest, and XGBoost.
____
III. ***Exploratory Data Analysis and Model Development***: EDA&MODEL.ipynb


In term of the *Model Development*: In order to develop the model, I’ve used the Supervised Machine Learning techniques to improve the process efficiency. Machine Learning models are able to learn from patterns of normal behavior. I’ve calculated the Accuracy Score on the training data and the R-Squared Score on the test data. Below is the result:
