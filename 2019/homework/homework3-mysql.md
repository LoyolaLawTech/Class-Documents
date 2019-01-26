# Homework 3

## Due Wednesday, January 30 at 5pm

Log on to MYSQL on our server. You should see that you have access to a new 
database called "Shared". Inside of that database you will see a table of NOPD 
use of force reports. Take a minute to browse this data and note what the 
fields are and how the data is arranged. 

To complete this homework, you will have to learn something new in SQL. In 
class we learned about the WHERE clause which allows you to put conditions on 
your search. You should now also know that you can put in more than one 
condition by using the AND keyword. So, for example, I can search two fields in 
this data with a query like this:

```mysql

SELECT * from nopd_use_of_force WHERE `Division level` = '2nd District' AND 
`Service Type` = 'Arresting';

```

Please answer the questions below by creating a file in your home directory 
called homework3. In answering the questions, please provide me with an answer 
along with the sql query or queries you used to arrive at your conclusion. You 
are free to use the mysql client, mycli, or phpmyadmin.

1. How many use of force reports occurred after January 1, 2018?
2. How many reports occurred in the year 2017?
3. Of the eight police districts, which one has the most use of force reports?  How many reports were there for that district?
4. How many of the use of force victims are said to have an "ethnicity" of 
   "black"? How many are "white"?


