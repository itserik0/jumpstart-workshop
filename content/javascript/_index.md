+++
title = "Javascript"
date = 2021-06-17T15:59:10-04:00
weight = 6
chapter = true
+++

# Javascript

## Javascript is like household appliances

![household appliances](images/appliances.jpg)

Unlike HTML or CSS, Javascript is a programming language. It is used by the browser to manipulate just about any element on a web page. 

## How do we add Javascript to a web page?

###  Internal Javascript

```
<script>

  // JavaScript goes here

</script>
```

### External Javascript

```
<script src="script.js"></script>
```

Like CSS the most desireable way to include javascript is through an external file. There are a number of reasons for this but the primary reasons are:
- Same file can be resused across multiple pages.
- Reduces the amount of code on a single page.
- Allows the browser to cache the file if which will speed up future page loads.

### Load the javascrtipt file last

Since the javascript tag is not visible to the user you'd think the ```<head>``` is a good place for it. However, a browser executes as it loads elements. So if the browser loads a javascript file that is meant to manipulate and element on the page that hasn't loaded yet there's a chance it will misfire and cause an error. A simple way to prevent this is to add the script tag at the end of your html document, just before the closing ```<body>``` tag.

Another, more advanced, way is to wrap your javascript in an event listener that will wait until the page has loaded before firing and javascript. That code looks something like this:

```
document.addEventListener("DOMContentLoaded", function(event) {
	// your javascript
});
```

## The DOM

Before we get into Javascript we need to understand the Document Object Model or DOM.

When a browser loads a page it puts a representation of the structure of the page's HTML elements into memory. This is the DOM. It is then represented an object-oriented representation of the web page, which can be modified with a scripting language such as JavaScript.

The DOM is not a programming language but a way of interfacing with programming languages. It's an API.

To access the DOM you don't have to do anything specific. It's done by the browser each time a web page loads.
