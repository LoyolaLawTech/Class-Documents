# Homework 2 - Due Wednesday, February 8 by 5pm.

For this homework, we our going to add some interactivity to our HTML by 
creating a form. Here is the HTML for the form we saw at the end of the last 
class:
```
<form name="test" action="https://loyolalawtech.org/class-exercises/test.php" method="post">
    <p>
    <label>First Name</label>
     <input type="text" name="fname">
    </p>
    <p>
        <label>Last Name</label>
    <input type="text" >
    </p>
    <p>
        <label>Favorite Color:</label>
    <select name="fav_color">
        <option value="">Please Select</option>
        <option value="red">Red</option>
        <option value="blue">Blue</option>
        <option value="green">Green</option>
        <option value="other">Other</option>
    </select>
    </p>
        <input type="submit" value="Go">
    </form>
```

You may want to actually type this form for practice and to see what it does.  
Pay attention to each line and make sure you know what it does. Notice that the 
form tag has an attribute "action" which contains a URL. This URL points to the 
script on the server which is going to handle the data you send. Also, notice 
each input has a "name" attribute.  When the form gets sent to the server, this 
name attribute tells the server the meaning of what the user has typed in the 
input. So, if the user types in "Smith" as the last name, the name of the field 
- "lname" - will get to the server along with "Smith" so that the server knows 
the last name is Smith, not the first name.

**Assigment**: You are going to make a simple calculator. Create a new form in 
JSbin with the "action" of "https://loyolalawtech.org/class-exercises/calc.php" 
Next, create two inputs, one with name "number1" and the other with the name 
"number2".  Then create a select with the name "operator" and  with three 
options: "add", "subtract", and "divide". Once you have done this, you should 
be able to submit your form to the server and get the result of this equation.  
If you get a response of "Invalid equation", this means there is a problem with 
your select. If you get a response of "Invalid data received", that means the 
server did not get all of your data. Check that all of your inputs have the 
correct "names" and that there are no other HTML errors.

*Note*: While you are testing your code in JSBin, you may notice that your output
panel gets stuck on the answer you received and you cannot get back to your form. 
The best thing to do it to open your output panel in a new tab by clicking on the
arrow in the upper right corner of the output panel. Then all you have to do is
reload the tab when you want to go back to your form. Good luck!
