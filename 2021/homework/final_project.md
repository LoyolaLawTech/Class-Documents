# Final Project (40 points)

# Due Wednesday May 19 by 5pm

The final project aims to synthesize everything you have learned in the clinic 
this semester. You will create a page that displays the eviction data from 
First Parish Court for the month of March, 2021. The best executed project will 
be used in the website the Clinic will use to advocate around post-COVID 
eviction issues.

To start your project, follow these steps:

1. Create a directory called final_project in your home directory.
2. Enter your final project directory and download the project skeleton by 
   executing:

```
    wget http://dev.loyolalawtech/~jmitchell/final_project.zip
    unzip final_project.zip

```

3. Install the necessary Node libraries by executing:

```
npm install

```

4. Create a database called final_project_data.db. Using 
   sqlite3, import the eviction data from final_project.csv into 
   that database. Check that your database is working by 
   executing some queries in sqlite3.

5. Configure index.js to work with your database. Ensure that you have at least 
   one route which, when requested in the browser, returns the whole database 
   as JSON.  (See below for extra credit opportunities here).

6. Start your API server:

```
forever start index.js
```

7. In your public_html directory, create a new directory called final_project.  
   Create two files index.html and index.js. Using HTML and jQuery, create a 
   page which makes an AJAX call to your API server and displays the eviction 
   data in a table. Make sure that your table has a header row with all the 
   columns correctly named. Use skeleton.css to style your table.

If you complete all of the steps above successfully with no errors, you will 
receive the full 40 points for this project. If you would like to receive extra 
credit, add some additional features. Here are some suggestions:

* Define additional routes in your index.js file. For example. 6. Start your * 
Define additional routes in your index.js file. For example, create a route 
that shows all evictions for a given zip code. For a real challenge, try 
creating a route that allows the user to search the database by first and last 
name. For hints on how to do this [consult this sample 
code](https://gist.github.com/judsonmitchell/2cc46a86f8b9dbe48c9e5613d51e4c7c) 
or look at the [Express.js 
documentation](https://expressjs.com/en/guide/routing.html).

* Add functionality to your table. For example, you can use the 
[dataTables](https://datatables.net/) library to add search and sorting 
functions to your table. 

* Use a different CSS library to add a different look to your table. For 
example, try using [Bootstrap](https://getbootstrap) or one of themed Bootstrap 
libraries at [Bootswatch](https://bootswatch.com/).

Up to 10 additional points of extra credit may be earned.

* You may not collaborate with any one else on this project. All work must be 
your own. You can consult your past Tech Clinic work, our class videos, and any 
internet reference sites. *
