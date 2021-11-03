# Data Modeling Cassandra

The purpose of this repo is to complete an ETL pipeline by creating tables in Apache Cassandra. The ETL pipeline transfers data from a set of CSV files within a directory, creates a streamlined CSV file to model and insert the data into Apache Cassandra tables.
The steps are as follows: 
- process the `event_datafile_new.csv` dataset to create a denormalized dataset
- model the data tables keeping in mind the queries you need to run
- load the data into tables created in Apache Cassandra and run the queries

## Datasets

One dataset: `event_data`. The directory of CSV files are partitioned by date. Here is an example of filepath to a file in the dataset: 
```
event_data/2018-11-08-events.csv
```

## Files

1. etl.ipynb
    * Jupyter notebook file used to create the tables and load data.
2. event_data
    * folder containing all the data files.
3. images
    * folder containing the images used in the ipynb file.
4. event_datafile_new.csv
    * file generated by the intermediate staging step in etl.
5. README.md

