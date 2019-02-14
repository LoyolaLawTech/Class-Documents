# Homework 5

## Due Monday, February 25 at 5pm
## Remember: NO CLASS on February 21

For this assignment, we are going to create a form to capture the data which 
you will be collecting at the self-help centers. Your form should be contained 
in a file called ai_form.html placed in your public_html directory.Your form 
will accept the data entered by the user and make a POST request to the 
following script on the server:

http://dev.loyolalawtech.org/~jmitchell/forms/ai_data.php

This script will in turn add your information to the "ai_test" table in our 
"shared" database.

Your form should include the following fields with the following 
characteristics:

1. A textarea with the name "narrative". It should be fairly large to allow a 
   lot of text.

2. A select with the name "classification1". The options should be every value 
   in the [National Subject Matter Index v.2 Family Law 
   section](https://nsmi.lsntap.org/browse-v2) , e.g "Adoption
   FA-01-00-00-00". Your select should submit only the code value, not the name 
   of the classification,  so e.g,

```html
   <option value="FA-01-00-00-00">Adoption FA-01-00-00-00</option>
```

3. Another select with the name "classification2". It should have the same 
   options as the classification1 select.

4. A text input with the name "reported_by". The value of this field should be 
   your name.

5. And, obviously, a submit button.

All of your inputs should have accompanying labels. Put some test data in your 
form and submit it.  The server should respond by telling you the data has been 
successfully received.  Then please log in to our database, and ensure that the 
data you submitted has been written to the ai_test table.

