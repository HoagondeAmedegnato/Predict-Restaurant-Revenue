# Predict-Restaurant-Revenue
***Its an assignment task to predict the revenue of restaurant***

![image](https://user-images.githubusercontent.com/79173300/152935398-39a4fc80-88dd-48f4-9f0c-a2977e648406.png)

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

In term of the *Exploratory Data Analysis*, I’ve examined and analyzed the dataset, and then proceeded to the visualizations. Several plots have been made, for example:

* I've analyzed the distribution of the revenue
![image](https://user-images.githubusercontent.com/79173300/152931804-4c2511f2-da72-4a92-a8f7-0a671900d701.png)

* I've counted by plot the feature "City Group"
![image](https://user-images.githubusercontent.com/79173300/152932138-0e92d044-92b5-4d7c-820b-b841e1aef5df.png)

* I've calculated the Correlation Matrix of the dataset, by selecting some variables
![image](https://user-images.githubusercontent.com/79173300/152932386-56f3e298-2934-4d01-91a8-ca27c2d1fecf.png)
Note that:

*There is a strong correlation of 0.97 between P9 and P12, which correlation is close to 1, means that there is a large positive relationship.*

*There is a strong correlation of 0.96 between P9 and P10, which correlation is close to 1, means that there is a large positive relationship.*

*There is a strong correlation of 0.93 between P10 and P12, which correlation is close to 1, means that there is a large positive relationship.*

*There is a correlation of -0.025 between P3 and revenue, which correlation is close to 0, means that there is no relationship.*

*There is a correlation of -0.028 between P5 and revenue, which correlation is close to 0, means that there is no relationship.*

*There is a correlation of -0.062 between P12 and revenue, which correlation is close to 0, means that there is no relationship.*



In term of the *Model Development*: In order to develop the model, I’ve used the Supervised Machine Learning techniques to improve the process efficiency. Machine Learning models are able to learn from patterns of normal behavior. I’ve calculated the Accuracy Score on the training data and the R-Squared Score on the test data. Below is the result:

![image](https://user-images.githubusercontent.com/79173300/152919740-7e3c7d0a-394e-4d35-ac88-a25be073263c.png)

**Conclusion in Selecting the Model**

I've received 100% Accuracy Score on Training data and -3.26% R-Squared Score on Test data in my "Predict Restaurant Revenue"; this means that:

* Logistic Regression and Support Vector Machines are the WINNERS, since they represent the highest score.
* In term of an accuracy score of the training data, both have the same score of 1.0 and in term of the R-Squared score on test data, Support Vector Machines scored -0.03260285700632415 and Logistic Regression scored -0.3594897101086121.
____
IV.	***Findings and Takeaways***

This project is made using the Supervised Machine Learning techniques, which give great predictions. But it's good to use the Unsupervised Machine Learning, such as Principal Component Analysis, K-Means, and some Deep Learning models.

____
***Medium Link***

A blog has been posted into medium as well. Follow this link:

https://amereine69.medium.com/predict-restaurant-revenue-7ce5afc82b6


