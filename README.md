# Vishnuvardhan-Task-Manager---Assessment
# AI Task Manager

## Project Explanation Video Link - https://vimeo.com/1082043454/d7b1c18c90?ts=0&share=copy

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

## Install Dependencies (In Jupyter Notebook)

         - pip install spacy pandas scikit-learn dateparser
         - python -m spacy download en_core_web_md

## Find the Source code in the "main" area repository named as "Task Manager Agent.ipynb"

###  How to Use (In Jupyter Notebook)
# Add a Task
     - add_task("Submit final report by tomorrow")
     -- Predict category and priority
        -- Extract a deadline
        -- Save to CSV and database
        -- Retrain the ML models

Automatically detects:

   -- Category: Work

   -- Priority: High

   -- Deadline: e.g. 2025-05-08

# View Tasks
     - view_tasks()
     - Shows all tasks with their category, priority, deadline, and status (e.g. Due Today, Overdue).

# Delete All Tasks
     - delete_all_tasks()
     - Clears all tasks from the database.



## How It Works
 --- spaCy detects date expressions like "tomorrow", "this evening"

 --- TF-IDF + Logistic Regression model is trained on labeled tasks to classify:
 
       -- Category (Work, Personal, etc.)
        
       -- Priority (High/Medium/Low)

--- SQLite stores tasks persistently

--- CSV keeps history for continuous retraining
