# Homework 2

## Due Wednesday, January 23 at 5pm.

This homework is simply a review of what we did in class this week. In your 
home directory, you will find two new files named data1.csv and data2.csv. This 
dataset is a collection of NOPD misconduct complaints which contains the nature 
of each complaint and its current status.

The second file is a copy of the first which * may or may not * have been 
modified.  Your homework is to answer a few questions about these files.  
Create a new file in your home directory named homework2 and answer the 
following questions:

1. Is data2.csv different than data1.csv? How? You can use either diff or 
   sha256sum to answer this question. Show me the command you entered to reach 
   your answer.

For the next questions, you should use the file data2.csv and the grep command:

2. If you browse through the data in data2.csv, you will see that the first 
   column is called "Incident Type" and there are two types of incidents. How 
   many are "Rank Initiated" (made by police supervisors) and how many are 
   "Public Initiated"?

3. You will also see there is a column called "Disposition". How many 
   complaints have been determined "Unfounded"?

Notes:

* If you are searching for a phrase with grep (in other words, more than one 
word with spaces between), you must surround the phrase with quotes.

* Search terms in grep are case-sensitive. "Unfounded" will return a different 
count than "unfounded"

* Each of you may have different copies of the file, so your answers may well 
differ from those of your classmates. 
