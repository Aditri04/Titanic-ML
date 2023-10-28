# Titanic-ML
Use machine learning to create a model that predicts which passengers survived the Titanic shipwreck


My Contribution
The training data had missing values in columns Age (177), Cabin (687) and Embarked (2) of 891 rows. I replaced the nulls in the Embarked column with the mode of the columns. Cabin feature has too many missing values to work with, hence i completely dropped this feature. To handle the missing values in Age column, I found that Pclass is highly correlated to Age. So i used Pclass  impute the missing age values. The Random Forest model only works with numerical data. I converted the categorical features such as Sex and Embarked into numerical value using the label encoder library. Next, i used the Name feature and extracted the Title of the person. I created 7 categories of the Titles. I used label encoder to convert it to numeric data. 

The test data too had missing values in Age, Cabin and Fare columns. I handled the missing values in Age the same way as the training data. Cabin feature is dropped. I filled the missing values in Fare column with its mean. Finally, I dropped the Ticket and PassengerId features because Ticket values were random and i could not figure out how to extract information from it. PassengerId was dropped because it does affect the survival of a passenger. 

I too used the Random Forest model and i got the accuracy score of 0.80224 on test data split from the train data. I could improve the Kaggle score to 0.78229

​