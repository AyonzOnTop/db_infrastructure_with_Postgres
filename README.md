# Project summary

## Purpose of Database
The database would serve a music streaming company, Sparkify. they would be able to query and analyze the data they've been collecting on songs and user activity on their new music streaming app. They particularly interested in understanding what songs users are listening to.

## Database schema design and ETL Pipeline
A **Star schema database** design model was used because it is particularly optimized for queries which is the main reason for the database

The function of the ETL pipelines is to extraect the data that resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

## How to run the Python scripts
* Run create_tables.py to create your database and tables.
* Run test.ipynb to confirm the creation of your tables with the correct columns
* Run etl.py to insert the song and log data into the created table.

## Explanation of the files in the repository

* test.ipynb displays the first few rows of each table to let you check your database.
* create_tables.py drops and creates your tables. You run this file to reset your tables before each time you run your ETL scripts.
* etl.ipynb reads and processes a single file from song_data and log_data and loads the data into your tables. This notebook contains detailed instructions on the ETL process for each of the tables.
* etl.py reads and processes files from song_data and log_data and loads them into your tables. 
* sql_queries.py contains all the sql queries, and is imported into the last three files above.

