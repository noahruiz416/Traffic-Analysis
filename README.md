# Traffic-Analysis Brief Overview
Summary: Traffic accident analysis using statistics and ML techniques to quantify and understand the factors that lead to a fatal or nonfatal traffic accident in the city of Tempe.

Purpose: Understand the leading causes of traffic accidents in Tempe and any weak areas are for the city in their traffic safety system.

Solution: Conduct an exploratory data anlysis to understand the underlying causes of traffic accidents in the City of Tempe and use ML to classify the servrity of an accident based on driver actions.

Data: The data for this project was sourced from a public database directly from the city of Tempe in Arizona. The data is from 2012 - 2020, and includes both fatal and nonfatal accident. Data was cleaned in python through the use of the pandas library, and pandasql was used for querying. Categorical data was also one hot encoded so that we can run it in our ML model.

Methods: Currently statistical tehcniques have been used such as the five number summary, histograms, pearsons correlation coefficient and regression modeling to explore the dataset. Implementation of classifcation tehcniques is currently in progress.

Model: For this project I used a random forest model, to classify the severity of a given traffic accident. Random Forest had the best performance in terms of accuracy comapred to SVM and logistic regression. Aditionally the use of RF allows our model to avoid common overfitting problems of decision trees, which I belive is a concern due to the large amount of categorical variables.

Feature Selection: In order to select relevant features, I used chi squared feature selection to find the features that our y variable (accident severity) is most dependent on. 

Basic Visualization With Tableau showing estimated injuries based on year, fatalities by year, Injuries by year and 7 most dangerous cross intersections:

<img width="813" alt="Screen Shot 2022-01-05 at 9 07 49 PM" src="https://user-images.githubusercontent.com/88412646/148326719-ae1c549f-8839-46e6-9184-bc0c3ae03b77.png">


# EDA Methods In Depth

Software: Python, Tableau Libraries Used: pandas, seaborn, pandassql, statsmodels

Purpose: Before working on the classification problem and working with the ML model, it is important to understand the underlying dataset that will be worked on throughout the length of the project. This documentation provides information on methods used for data exploration / analysis and also provides examples on how to run certain functions.

Data: As stated in the readme our data was sourced from the city of tempe and contains information regrading traffic accidents from 2012 - 2020.

Exploring the data: Pandas and Seaborn were the main libraries used for visualizing and storing our data on top off that pandassql was also very helpful for this project. If you are unfamiliar with pandasql, there is more info here: but essentailly it allows users to write sql queries to clean and query whole pandas dataframes.

Data Exploration Continued: First I used pandasql, to count the total number of accidents occuring form 2012 - 2020, shockingly there was a slow upward trend in the amount of accidents occuirng until a huge drop occured in 2020, dropping by more than 50%. After that pandasql was used ot split datasets into Fatal and Non - Fatal datasets. I decided to do this just so I can get a better idea of what was occuring in fatal and nonfatal accidents. We then use the upper and lower limits of our dataset to remove any outliers, that have to do with the age of accident drivers, I did this because there was a large amount of drivers who were labeled to be 200 years old. Finally we end the majority of our exploration with simple histograms to understand age, and year distributions and heatmpas to look at various other realtionships within the dataset.
