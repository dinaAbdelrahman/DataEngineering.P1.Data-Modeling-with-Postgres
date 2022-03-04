# Introduction
Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app.

# Data structure
The available data consists of 2 parts:
a directory of JSON logs on user activity on the app (which songs were requested by users, the log timestamp, some users information ) --> operational database which gets update by users transactions
a directory with JSON metadata on the songs in their app (songs information as well as artists) --> static database which is updated in case the startup increases its catalogue


In order to prepare the data for analytics, we should design the data into facts and dimensions tables in star schema. This would help data analysts to easily explore the data and uncover some insights.

## ERD diagram



# Project Steps:
1.I first prepared my ERD, defined the columns data types and created the tables. --> please check attached ERD <br />
2.Created the tables as well as the insert statment in sql_queries.py <br />
3.Run create_tables.py to drop and create the tables <br />
4.for single file processing, etl.ipynb reads and processes a single file from song_data and log_data and loads the data into the tables. This is useful to troubleshoot each single step of data extraction, transformation and finally loading on the Sparkify database<br />
5.transfer the same the code in etl.ipynb to etl.py to process the whole logs and songs data<br />
6.I run the test.ipnb to confirm proper loading for the data in all tables.
