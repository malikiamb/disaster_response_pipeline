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


## Notice classification results of search for relief aid in Barbados

### Webpage Visual
<img width="694" alt="Message Classification Example" src="https://user-images.githubusercontent.com/75813316/184791030-1d4e19cc-11e1-427e-b1f2-0fdb2a02906b.png">

## Execution:
You can run the following commands in the project's directory to set up the database, train model and save the model.

To run ETL pipeline to clean data and store the processed data in the database python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/disaster_response_db.db

To run the ML pipeline that loads data from DB, trains classifier and saves the classifier as a pickle file python models/train_classifier.py data/disaster_response_db.db models/classifier.pkl

Run the following command in the app's directory to run your web app. ## python run.py

## HTML App Here

https://052b8c06e71c40e99045311a7e35ff96-3000.udacity-student-workspaces.com/

## Additional Visuals
<img width="917" alt="Visual A " src="https://user-images.githubusercontent.com/75813316/184790548-e3fbaf06-5717-4054-8d5f-6620d92a2a3b.png">

# Improve classification model for future reference
#### Steps to improve model beyond current status for better outcome

https://neptune.ai/blog/improving-machine-learning-deep-learning-models

## Resources

Classifier Models

https://medium.com/fuzz/machine-learning-classification-models-3040f71e2529#:~:text=There%20are%20a%20number%20of,%2Drest%2C%20and%20Naive%20Bayes.

What is natural language processing?

https://en.wikipedia.org/wiki/Natural_language_processing



