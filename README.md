# Movies_ETL

Extract, Transform & Load

## Objectives

* Create an automated ETL pipeline.

* Extract data from multiple sources

  - Wikipedia
  - Kaggle
  - MovieLens
  
* Clean and transform the data automatically using Pandas and regular expressions.

* Create new tables by loading newly created Dataframes into PostgreSQL


## Summary

* A function was created that took in three arguments: Wikipedia Raw Data, Kaggle Metadata, and MovieLens Rating Data (Kaggle)

Then I used the code I wrote during the module's lesson and applied it to the function, so that the function would perform all of the transformation steps. I also added the lesson code I wrote for the load steps and applied it to the function. I confirmed the function worked correctly on the current Wikipedia and Kaggle data.

Several assumptions are being made in this automated ETL pipeline.

The uploaded data will stay in the same formats:

Wikipedia data in JSON format.

Kaggle metadata and rating data in CSV formats.

There are null or mostly null columns that need to be removed.

The list of 'alternate titles' is valid.

There will not be any new 'alternate titles' added to the data.

The data types will be correct when loaded into SQL.

When creating regular expressions for budget and box office figures, we need to capture 'million' and 'billion' as expressions.







