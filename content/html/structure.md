+++
title = "The Complete Structure"
date = 2021-06-17T16:34:21-04:00
weight = 4
+++

## A complete HTML document

At the highest level of a web document are the ```<html>```, ```<head>```, and ```<body>``` tags. As you noticed from the earlier HTML examples these tags are optional to render HTML, but they are highly semantic and help organize your document. 

```
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <h1>My First Heading</h1>
        <p>My first paragraph.</p>
    </body>
</html> 
```

### The DOCTYPE

The ```<!DOCTYPE html>``` declaration defines that this document is an HTML5 document. HTML5 is the latest (and in theory the last) set of HTML specifications. The HTML5 specifications are "living standars" which mean they are constantly evolving.

### HTML

The ```<html>``` element is the root element of an HTML page.

### HEAD

The ```<head>``` element is a container for metadata. HTML metadata is data about the HTML document. Metadata is not displayed.

The HTML ```<head>``` element is a container for the following elements: ```<title>, <style>, <meta>, <link>, and <script>```.

### Title

The ```<title>``` element defines the title of the document. The title must be text-only, and it is shown in the browser's title bar or in the page's tab.

The ```<title>``` element:

- defines a title in the browser toolbar
- provides a title for the page when it is added to favorites
- displays a title for the page in search engine-results

### Style

The ```<style>``` element is used to define style information (CSS) for a single HTML page. More on this later.

```
  <style>
      body {background-color: white;}
      h1 {color: red;}
      p {color: blue;}
  </style> 
```

### Link

The ```<link>``` element is how you include external files. This is used mostly for stylsheets (CSS) but also for fav icons and app icons for homescreen apps on mobile devices.

```
<link rel="stylesheet" href="mystyle.css"> 
```

### Meta

The ```<meta>``` tag defines metadata about an HTML document. Metadata is data (information) about data.

Here are some common examples:

```
<meta charset="UTF-8">
<meta name="description" content="This webpage is about Beanie Babies">
<meta name="keywords" content="Beanie Babies are a line of stuffed toys.">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta http-equiv="refresh" content="5" />

```

The list of possible meta tags is too long to go into in this workshop. Here's an exhaustive list from the NC State University Library website.

```
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
<meta property="fb:app_id" content="251756438193216" />
<meta property="og:title" content="" />
<meta property="og:description" content="The NC State University Libraries is the gateway to knowledge for the North Carolina State University community and partners." />
<meta property="og:type" content="website" />
<meta property="og:url" content="https://www.lib.ncsu.edu/node" />
<meta property="og:image" content="https://www.lib.ncsu.edu/themes/custom/ncsulibraries/images/screenshot.jpg" />
<meta property="og:image:alt" content="NC State University Libraries Logo" />
<meta name="twitter:description" content="The NC State University Libraries is the gateway to knowledge for the North Carolina State University community and partners." />
<meta name="twitter:title" content="" />
<meta name="twitter:site" content="@ncsulibraries" />
<meta name="twitter:card" content="summary_large_image" />
<meta name="twitter:image" content="https://www.lib.ncsu.edu/themes/custom/ncsulibraries/images/screenshot.jpg" />
<meta name="twitter:image:alt" content="NC State University Libraries Logo" />
<meta name="description" content="The NC State University Libraries is the gateway to knowledge for the North Carolina State University community and partners." />
<meta itemprop="description" content="The NC State University Libraries is the gateway to knowledge for the North Carolina State University community and partners." />
<meta itemprop="name" content=" | NC State University Libraries" />
<meta name="google-site-verification" content="vxwfJngqcuxRLZV58ZE38_-_fgcEf3eCqy5aMIp8oGA" />
```