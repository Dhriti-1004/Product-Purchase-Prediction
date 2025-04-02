# Product-Purchase-Prediction
Machine learning model to predict whether a customer will buy the product or not

Source of dataset: Kaggle
It contains 400 rows and 5 columns:
User ID, Gender, Age, EstimatedSalary, Purchased     
Using pandas, this data was loaded into a dataframe and its basic information was studied. Many insights about the data were found during Exploratory Data Analysis (EDA) and the impact of all the columns on the output were studied. The data was found to be divisible by lines parallel to x and y axes, with estimated salary and age being the splitting columns.
# Data preprocessing:
The categorical columns were converted into numbers so that the data becomes suitable for training. Minmax scaling was done to improve the model performance.
# Models trained:
1) Decision Tree: it was the most intuitive model looking at the scatterplots of the data which suggested that the data was separable using different columns. It gave an cross validation score of 0.89 without any tuning.
2) Random Forest: with decision trees as their base, these were expected to give a good performance. With a cross validation score of 0.88, decision trees performed better and so were chosen.
3) GridSearchCV: with Decision Trees as the algorithm, these were tuned to improve performance. The best model had a cross validation score of 0.91.




