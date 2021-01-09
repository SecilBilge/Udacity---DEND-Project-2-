# Project 2 - Data Modeling with Apache Cassandra

The Sparkify initiative wants to analyze user activities using songs and user data. 
Existing data is stored in CSV files. This makes it difficult to query and analyze.

## Getting Started

This project creates an ETL pipeline by loading all from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.

### **Datasets**
There is one dataset: `event_data`. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:

```
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv

```

Sample Record :
![Eventdata](example_eventdata.png)


## Files:
1.  Project_1B_ Project_Template.ipynb displays all logical opearation
2.  Event_data directory of CSV files partitioned by date 


## Prerequisites

*   Python 3.6 (or above https://realpython.com/installing-python/)
*   Apache Cassandra  (https://cassandra.apache.org/download/)
*   Jupyter Notebook  (https://jupyter.org/install)

## Database Model

Designing tables to answer these queries:
*   Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
![1](1.png)

*   Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
![2](2.png)

*   Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'
![3](3.png)


## Installing

1) Run "Project_1B_ Project_Template.ipynb" Part I. ETL Pipeline for Pre-Processing the Files
2) Run Part II. Complete the Apache Cassandra portion of the project after first step you are ready to work with the CSV file titled "event_datafile_new.csv"

## Tests
With Jupyter you can test every step seperately as follows:

*   You can test every step of getting data from tables into Project_1B_ Project_Template.ipynb

## Results

1) Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
Faithless Music Matters (Mark Knight Dub) 495.30731201171875

2) Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
Down To The Bone Keep On Keepin' On Sylvie Cruz 0
Three Drives Greece 2000 Sylvie Cruz 1
Sebastien Tellier Kilometer Sylvie Cruz 2
Lonnie Gordon Catch You Baby (Steve Pitron & Max Sanna Radio Edit) Sylvie Cruz 3

3) Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'
Jacqueline Lynch
Tegan Levine
Sara Johnson

## Authors

* **Secil Bilge** - *Data Engineering NanoDegree Second Project* - (https://github.com/SecilBilge)


