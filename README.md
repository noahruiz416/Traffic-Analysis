# Traffic-Analysis (In Progress)
Summary: Traffic accident analysis using statistics and ML techniques to quantify and understand the factors that lead to a fatal or nonfatal traffic accident in the city of Tempe.

Purpose: Understand the leading causes of traffic accidents in Tempe and any weak areas are for the city in their traffic safety system.

Data: The data for this project was sourced from a public database directly from the city of Tempe in Arizona. The data is from 2012 - 2020, and includes both fatal and nonfatal accident. Data was cleaned in python through the use of the pandas library, and pandasql was used for querying. Categorical data was also one hot encoded so that we can run it in our ML model.

Methods: Currently statistical tehcniques have been used such as the five number summary, histograms, pearsons correlation coefficient and regression modeling to explore the dataset. Implementation of classifcation tehcniques is currently in progress.

Model: For this project I used a random forest model, to classify the severity of a given traffic accident. Random Forest had the best performance in terms of accuracy comapred to SVM and logistic regression. Aditionally the use of RF allows our model to avoid common overfitting problems of decision trees, which I belive is a concern due to the large amount of categorical variables.

Feature Selection: In order to select relevant features, I used chi squared feature selection to find the features that our y variable (accident severity) is most dependent on. 

Basic Visualization:

<img width="441" alt="Screen Shot 2022-01-05 at 9 02 30 PM" src="https://user-images.githubusercontent.com/88412646/148326656-859dc362-96db-4c25-8b91-3f939297ad45.png">


<img width="646" alt="Screen Shot 2022-01-05 at 9 05 28 PM" src="https://user-images.githubusercontent.com/88412646/148326632-578895fb-e141-4579-b23a-5abac3015778.png">

<img width="606" alt="Screen Shot 2022-01-05 at 9 05 33 PM" src="https://user-images.githubusercontent.com/88412646/148326637-8cdcffb0-c86b-4795-9ed7-d38c55aa0de7.png">

<img width="870" alt="Screen Shot 2022-01-05 at 9 05 21 PM" src="https://user-images.githubusercontent.com/88412646/148326642-db51b8b4-19a1-42b7-b8b7-d4946a4e5adf.png">

