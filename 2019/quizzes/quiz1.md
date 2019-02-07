# Quiz 1

## 30 minutes

Assume that you are defense counsel in a murder case and reviewing discovery. 
Your client is alleged to be an accessory after the fact to the murder. Her 
boyfriend, who she calls "Zaddy" is alleged to be the shooter. The NOPD 
executed a search warrant on your client's phone when she was arrested. Please 
do the following:

1. Log on to our server and create a new directory called "quizzes" in your 
   home directory.

2. Inside the quizzes directory, create a new file called "quiz1". You will use 
   this to provide your answers.

3. Next you must download the dump of your client's call logs which have been 
   "provided" to you by the NOPD. To do this, use the wget command, which will 
   get the file off of the loyolalawtech server and put it in on our current 
   one:

```bash

    wget https://loyolalawtech.org/phone_dump.csv

```

4. In the discovery documents, the NOPD forensic analyst says the sha256 hash 
   of the call log is 
   5f3712d0ee15c75e91cbc3e2e7b70a204635f0871587164c9fc1274ae08cb369.
   Answer this question "yes" or "no" and tell me how you decided your answer: 
   
   a. Has the copy you just downloaded been modified or tampered with in any 
   way?

5. I have imported the call log you received into our MYSQL shared database. 
   Log on the database and look for the "phone_dump" table in the "shared" 
   database. Take a minute to look at the data and see how it is structured.  
   Next answer these questions:

   a. How many calls did your client receive from the shooter "Zaddy" overall 
   in this dataset? Note that Zaddy has more than one phone number.

   b. The murder is alleged to have taken place on May 1, 2017. Did your client 
   call Zaddy on the day of the murder? If so, how many times?

   c. Did Zaddy call your client on the day of the murder? If so how many 
   times?

Write your answers to these questions in your quiz1 file. Please show the MYSQL 
queries you used to reach your conclusions.

## Hint:

In MYSQL, you can do a wildcard search by using the LIKE %[search term]% 
syntax.  So, for example, if I'm trying to find all calls in this dataset which 
originated on April 29, and I execute the following query:

```sql

SELECT * from phone_dump where `Time` = '29-Apr';

```

I will get zero results because MYSQL tries to match all of the data in the 
field not just part of it. To search for fields where only part of the data 
contains '29-Apr', I would do:


```sql

SELECT * from phone_dump where `Time` LIKE  '%29-Apr%';

```

##

Note: Everything in this quiz is graded for accuracy. Your quizzes directory 
and quiz file must be in the right place, and your answers to the data 
questions must be correct. All answers should be your own work.
