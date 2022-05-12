# udacity--de-data-modelling-postgres

	<h1>Data Modelling with Postgres</h1>

<h2>Background:</h2>

Sparkify want to analyse data that they have collected on songs and user activity. They would like insights on the songs that their users are listening to.


<h2>Project Aims:</h2>

- Create a database Star Schema
- Build an ETL pipeline using Python


<h2>Database Schema:</h2>

The database I designed used a Star Schema as this allows for denormalised tables and simplified queries. The Schema included one Fact Table (the songplays table) and four Dimension Tables (songs, artists, users, time).

Each Dimension Table has a Primary Key:

- users Table: user_id (PRIMARY KEY)
- songs Table: song_id (PRIMARY KEY)
- artists Table: artist_id (PRIMARY KEY)
- time Table: start_time (PRIMARY KEY)

(Diagram of Start Schema found in the 'Start Schema.png' file)


<h2>Project Files & Steps</h2>

- README.md
- sql_queries.py includes all the sql queries used in this project
- create_tables.py creates the tables; this file needs to be rerun each time a change in the ETL files is made
- etl.py reads and processes files from song_data and log_data and loads them into your tables. You can fill this out based on your work in the ETL notebook.
- etl.ipynb reads and processes a single file from song_data and log_data and loads the data into your tables. This notebook contains detailed instructions on the ETL process for each of the tables.
- test.ipynb displays the first few rows of each table to let you check your database.


To run the project, first run the create_tables.py in a new Terminal using the command 'python create_tables.py'. Once this is complete, run the command 'etl.py' in the same Terminal. To check that the tables have been created successfully, you can then run the test.ipynb file.
    
