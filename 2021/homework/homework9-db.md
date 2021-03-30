# Homework 9 - Databases
## Due April 14 by 5pm

Create a file in your dbs/ directory called homework.db. Import the following 
cvs file to your dbs directory by running:

```bash
curl https://data.nola.gov/api/views/uiry-as9x/rows.csv?accessType=DOWNLOAD > abo.csv

```

This is a CSV file from the City of New Orleans which tracks licensed alcoholic 
beverage outlets in the city. We will use it to practice some SQL. Import the 
csv file into sqlite3 and create a table called outlets. 

Once you have successfully created the database, create a file in your dbs/
directory called answers.txt. Using SQL queries, answer the following questions 
and put your answers in your answers.txt file. ** Please show the SQL query you 
used to get the answer along with the answer**.

1. Which zip code has more ABOs, 70115 or 70118? Give the number of ABOs in 
   both zip codes.
2. What is the latitude and longitude of Fat Harry's?
3. How many ABOs are there on Oak Street?
 
If you need help, please review the recording of our class. You can also 
consult 
[this](https://www.codecademy.com/learn/learn-sql/modules/learn-sql-queries/cheatsheet) 
or any other mysql cheat sheet online.
