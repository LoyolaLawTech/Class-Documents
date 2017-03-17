# Homework - AJAX

## Due Wednesday, March 22 by noon.

For this homework, create an AJAX query that sends a POST request to our 
address "database" at  https://loyolalawtech.org/json/address.php. The database 
has only three names in it: Jane, Fred, and Michelle. Your query should be an 
object with the key "search" and one of these names as a value. HINT: Something 
like this will be somewhere in your AJAX request:

```js
data: {'search': 'Michelle'}
```

The data which you get back from the server should be a JSON object with the 
person's full name, address, city, state, and zip code.  Put this data in an 
HTML document as a properly formatted address. In order to get your address to 
display nicely, you will likely want to use jQuery's 'append' function and 
possibly some line break tags, like so:

```html

Name <br />
Address <br />
City, State, Zip
```
