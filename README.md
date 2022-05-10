# Disaster-Response-Pipeline
Disaster Response pipeline is a data ETL, processing, modeling project in Udacity Data Science Course. The raw dataset we will use contain 26k message in Twitter and contaent tag to help developer to distinguish message in right category. During this project, we will build a classifier model to help organizztions filter the most important message to rescure people who still in trouble.

Inorder to accomplish this project, I used several packages which listed below:
1.pandas
2.numpy
3.nltk (Bag of Words (BOW))
4.sqlalchemy (SQLite in Python)
5.sklearn (Grid Search Cross Validation Random Forest Classifier K nearest neighbors (KNN))


# Data

The data files associated with this project are from Figure Eight

messages.csv: FIgure Eight provide 26,248 messages
categories.csv: Raw categories data, total 36 categories.

# Project Process

#1.ETL Pipeline

Loads messages and categories dataset

Clean data

Feature Engineering

Stores it in a SQLite database




#2.ML Pipeline

Loads data from the SQLite database

text processing and machine learning pipeline

Trains and tunes a model using GridSearchCV

Exports the model


#3.Build web app

Create HTML templates

Build Flask web application



- app
| - template

| |- master.html  # main page of web app

| |- go.html  # classification result page of web app

|- run.py  # Flask file that runs app


- data
- 
|- disaster_categories.csv  # data to process 

|- disaster_messages.csv  # data to process

|- process_data.py

|- InsertDatabaseName.db   # database to save clean data to

- models
|- train_classifier.py

|- classifier.pkl  # saved model 


# Result Images
![Message Genre Scatter Plot (Training)](https://user-images.githubusercontent.com/98485051/167718906-c80a5579-8c60-404e-8619-1129fc274a2f.png)
![Result](https://user-images.githubusercontent.com/98485051/167719050-cd1e7c3f-c73a-4c7c-a21b-1491c50c13c7.png)
