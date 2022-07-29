+++
title = "CSS"
date = 2021-06-17T15:50:06-04:00
weight = 5
chapter = true
+++

# CSS

CSS stands for **Cascading Style Sheets**. CSS is a style sheet language used for describing the presentation of a document written in HTML. It was designed to enable the separation of presentation and content. 

If HTML is like lumber, then CSS is interior decorating. 

![interior decorating](images/interior-decorating.jpg)

## Why CSS?

Separating the style of a webpage from it's content is very important. When tags like ```<font>```, and color attributes were added to HTML 3 (we're currently on HTML 5), it increased the possibilites for styling a web site without using CSS, but it was a nightmare for web developers. Development of large websites, where fonts and color information were added to every single page, became a long and arduous process.

### Avoid duplication. 
If you add style attributes to each HTML element you would have to write the same styles over and over again. 

```
<font color="red" face="Verdana, Geneva, sans-serif" size="+1">This is my first paragraph.</font>
<font color="red" face="Verdana, Geneva, sans-serif" size="+1">This is my second paragraph.</font>
``` 

With CSS you can write something like the following, and it will apply to all of your ```<p>``` that include that style:

#### CSS
```
p{
    color: red;
    font-family: Arial;
    font-size: 16px;
}
```

### More attributes

The old style attributes and tags were limited to a few properties like color, font, font size, width, height, and a few others. Modern CSS now has ~520 properties and counting.


### Smaller file size

Including a CSS style sheet allows your broswer to cache the file at the beginning of your session instead of loading all this markup each page load.