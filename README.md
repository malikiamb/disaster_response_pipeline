# Disaster Response Pipeline Udacity

# We will build a classifier model that evaluates and classifies results of messages sent during a disaster

## Project Description

Utilizing data from Appen, we will Extract, Transform and Load as a first step. 
There are 2 data files:
messages.csv and categories.csv

## Notebook : ETL Preparation
  Explore structure of data
  Merge both csv's
  Create new category names
  Convert category values to Binary Values
  Remove Duplicates 
  Save new df to sqlitedatabase using Pickle
  
## Notebook ML Pipeline
  Load sql data
  Write Tokenizer to process text data
  Build Machine Learning Pipeline
  Train Pipeline
  Test Model
  Evaluate F1 Score, Accuracy, Precision & Recall
  Utilize Gridsearch to improve model
  Export final model as pickle file
 

## File Structure:
- app
| - template
| |- master.html  # main page of web app
| |- go.html  # classification result page of web app
|- run.py  # Flask file that runs app

- data
|- disaster_categories.csv  # data to process 
|- disaster_messages.csv  # data to process
|- process_data.py
|- InsertDatabaseName.db   # database to save clean data to

- models
|- train_classifier.py
|- classifier.pkl  # saved model 

- README.md

## HTML App Here

https://052b8c06e71c40e99045311a7e35ff96-3000.udacity-student-workspaces.com/
