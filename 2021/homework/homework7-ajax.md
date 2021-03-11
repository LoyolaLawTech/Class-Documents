# Homework 7 - AJAX

## Due March 17 at 5pm

For this assignment, create two files in your public_html folder: ajaxhm.html 
and ajaxhm.js. Load an image in your HTML file. Put a button under it that, 
when clicked, replaces it with another image. [Here's an 
example](https://drive.google.com/file/d/1q_nt7TZO1GdzBWrPK8SMTr0NHz-RCGmP/view)

### TIP:

You can use any image you want. Remember that in HTML you can load an image by 
putting a URL or a file name in the src property of the img tag.  If you want 
to load a copy of your image onto the server use the tool wget. Here is how is 
how I got the image I used in the demo. In my terminal, while in my public_html 
directory, I did: 

```bash

wget https://cdn.whereyart.net/original/jackson_square_twilight_2016-02-02-20-39-42.jpg
mv jackson_square_twilight_2016-02-02-20-39-42.jpg img1.jpg

```

As you can see, I called wget followed by the URL of the file. It downloaded 
the file to my public_html directory. I changed the name from the long 
jackson_square, etc to just img1.jpg.  I then loaded that in in my image tag 
like so:

```html
<img src="image1.jpg">
```


