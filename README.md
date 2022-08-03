# Movies_ETL

An exercise in performing an Extract, Transform, Load (ETL) process to create data pipelines using Python, Pandas and PostgreSQL using very large data files.

![ETLGraphic](https://github.com/rloufoster/Movies/commit/90bf9d99f19ace46dce7a3bf7f78869c17cf04f3)


## Objectives

The purpose of this project was to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables that is connected to a database. The chosen topic is all about Movies from 1990 to 2018 and combining the information from 3 different resources.

## Method

Create an ETL pipeline using Jupyter Notebooks and PostgreSQL from raw data to SQL database.

*  **Extract:** Collected data from multiple sources using Python in Jupyter Notebook.
        * Wikipedia: format- .json, file size: 6.2MB), 7,311 movie titles and information about the movies.
        * Kaggle: 2 files (format: .csv)
            * a metadata file from [The Movie Database](https://www.themoviedb.org/) containing movie details with 45.5 thousand entries. (File size: 34.4MB) 
            * a dataset from [MovieLens](https://movielens.org/) containing over 26 million movie ratings/review. (File size: 709.6MB)

* **Transform:** Clean and structure data using Pandas and regular expressions (RegEx) to achieve desired form. (i.e. using RegEx to 
    parse data and transform text into numbers.
        * Deleting bad data (corrupted or missing), removing duplicate rows, and consolidating columns.
        * Using RegEx to parse data and transform text into numbers

* **Load:** Export transformed data into an ProgresSQL Database using PQAdmin.

## Results

After cleaning and merging, two new tables were created using Python in Jupyter Notebook and exporting the tables into PostgreSQL.  

**Movies Table**

![movies1_query_table](https://github.com/rloufoster/Movies/blob/main/movies_query.png)



**Ratings Table**

![ratings_query_table](https://github.com/rloufoster/Movies/blob/main/ratings_query.png)
























