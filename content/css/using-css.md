+++
title = "Using CSS"
date = 2021-06-17T16:34:21-04:00
weight = 2
+++

## Using CSS

CSS can be added to an HTML documents in 3 ways:

### 1. Inline

By using the style attribute inside HTML elements

```
<h1 style="color:red;">A Red Heading</h1>
<p style="color:pink;">A pink paragraph.</p> 
```

### 2. Internal
By using a ```<style>``` element in the ```<head>``` section

```
<!DOCTYPE html>
<html>
    <head>
        <style>
            body{
                background-color: orange;
            }
            h1{
                color: blue;
            }
            p{
                color: #cc0000;
            }
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html> 
```

### 3. External

By using a ```<link>``` element to link to an external CSS file.

```
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html> 
```

The external style sheet can be written in any text editor. Save the file with a .css extension.

There's no need for the ```<style>``` tag in you CSS file since it doesn't accept HTML. Just add the following:

```
body{
    background-color: orange;
}
h1{
    color: blue;
}
p{
    color: red;
}
```

## Which is best?

![CSS Meme](../images/css-meme.jpg)

An external CSS sheet is the best for a few reasons:
- One file for many pages. If you use internal CSS you would need to add a huge block of CSS code to each page. Simply including the link to the stylsheet is much simpler. You can also only edit the CSS in one place and the changes will cascade down to each page. 
- Seperate file will be cached and will increase the efficincy of page loading. 