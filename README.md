# Vishnuvardhan-Task-Manager---Assessment
# AI Task Manager

This is an AI-powered Task Manager that understands your tasks written in natural language (like "Submit report by Friday") and automatically:

- Classifies them into categories like Work, Personal, Errand, or Learning
- Predicts priority (High / Medium / Low)
- Extracts deadlines from text using natural language processing
- Stores tasks in a local database and CSV file for future referance

## Features

- Smart task categorization
- Priority detection using Machine Learning
- Deadline extraction using NLP (like “tomorrow” or “next Monday”)
- Saves tasks to a SQLite database
- Learns continuously from new tasks

## To Run the Project (In Jupyter Notebook)
-- Import the following requirements
     - pip install spacy pandas scikit-learn dateparser
     - python -m spacy download en_core_web_md

### How to Use (In Jupyter Notebook)
## Find the Source Code Run them all and then 

1). Add a Task  
       --- add_task("Prepare slides by end of today")

        -- Predict category and priority
        -- Extract a deadline
        -- Save to CSV and database
        -- Retrain the ML models

2). View Tasks
       -- view_tasks()
        See all tasks with their deadlines and whether they’re due, overdue, or upcoming.

3). Delete All Tasks
       -- delete_all_tasks()
        This will clear the database. Use with care.

## How It Works
 --- spaCy detects date expressions like "tomorrow", "this evening"

 --- TF-IDF + Logistic Regression model is trained on labeled tasks to classify:
 
       -- Category (Work, Personal, etc.)
        
       -- Priority (High/Medium/Low)

--- SQLite stores tasks persistently

--- CSV keeps history for continuous retraining



