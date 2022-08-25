# Movies-ETL

This project was focused around the concepts of Extract, Transform and Load processes, known as ETL. The data from Wikipedia, Kaggle and aggregated ratings were utilized to create a movie database from a clean dataset for a fictional Hackathon. 

To accomplish this, the ETL process is used to extract the Wikipedia and Kaggle data from their files, and next transform the dataset by cleaning the rows and formatting datatypes, performing joins, and loading the cleaned dataset into PostgreSQL database.

## Overview
We configured an automated pipeline that inputs new data, from Wikipedia data, Kaggle metadata and the MovieLens rating data, for the Hackathon. Then we transformed the data and loaded the data into an existing PostgreSQL database.

For this analysis we performed the following:
1. Write an Extract, transform, and load function to read three data files
2. Extract and transform the Wikipedia data
3. Extract and transform the Kaggle and rating data
4. Load the data to a PostgreSQL Movie Database.
	
This process was accomplished by using four Jupiter notebooks. The details are provided below:

## Results

### First, the ETL function is written to read three data files
Where the function inputs the Wikipedia JSON, Kaggle metadata and MovieLens csv files and ultimately creates three separate DataFrames which we later use.
<br/>
### The Wikipedia data is extracted and transformed.
The TV shows are filtered and the redundant data is consolidated, also in addition to that any duplicates are removed as well, lastly formatted the Wikipedia data


<br/>
### The Kaggle and rating data is extracted and transformed.
Same as before the redundant data is consolidated, the duplicates is removed, and the data is formatted and grouped. Then all the  data is merged with the Kaggle and rating data, with the Wikipedia movies Dataframe.
<br/>
### PostgreSQL is used and the data is loaded into the Movie database.

### Summary
The ETL function is utilized to create, gather and clean movie data from multiple sources. It also transforms and merges data, loads it into PostgreSQL ,and then put into tables that are ready to use for the Amazing Prime Hackathon.
