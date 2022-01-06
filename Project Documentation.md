# EDA Documentation

Software: Python, Tableau 
Libraries Used: pandas, seaborn, pandassql, statsmodels

Purpose: Before working on the classification problem and working with the ML model, it is important to understand the underlying dataset
that will be worked on throughout the length of the project. This documentation provides information on methods used for data exploration / analysis 
and also provides examples on how to run certain functions.

Data: As stated in the readme our data was sourced from the city of tempe and contains information regrading traffic accidents from 
2012 - 2020. 

Exploring the data: Pandas and Seaborn were the main libraries used for visualizing and storing our data on top off that pandassql
was also very helpful for this project. If you are unfamiliar with pandasql, there is more info here:
but essentailly it allows users to write sql queries to clean and query whole pandas dataframes. 

Data Exploration Continued: First I used pandasql, to count the total number of accidents occuring form 2012 - 2020, shockingly
there was a slow upward trend in the amount of accidents occuirng until a huge drop occured in 2020, dropping by more than 50%. 
After that pandasql was used ot split datasets into Fatal and Non - Fatal datasets. I decided to do this just so I can get a better idea
of what was occuring in fatal and nonfatal accidents. We then use the upper and lower limits of our dataset to remove any outliers, that have 
to do with the age of accident drivers, I did this because there was a large amount of drivers who were labeled to be 200 years old.
Finally we end the majority of our exploration with simple histograms to understand age, and year distributions and heatmpas to look at various 
other realtionships within the dataset.
