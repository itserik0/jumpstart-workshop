+++
title = "HTML"
date = 2021-06-17T15:59:10-04:00
weight = 3
chapter = true
+++

# HTML

HTML stands for _Hyper Text Markup Language_. HTML provides a way of creating structured documents. These documents are built with elements delineated by tags. 

## HTML is like lumber

![html is like lumber](https://imagesvc.meredithcorp.io/v3/mm/image?url=https%3A%2F%2Fstatic.onecms.io%2Fwp-content%2Fuploads%2Fsites%2F23%2F2022%2F02%2F14%2Fbuy-land-build-house-2000.jpg)

HTML is used to construct a web page, not style or manipulate it. That will come later. 

HTML is not a programming language, it's a markup language made up of tags, also called elements, like ```<div>``` or ```<span>```. 

Each of these ~142 elements are written using angle brackets. Tags such as ```<p>``` surround content 
```
<p>some text</p>
```
and provide information about document text and may include other tags as sub-elements 
```
<div>
    <h1>Page Title</h1>
</div>
```
These tags can be used for content such as headings, paragraphs, lists, links, quotes and other items. Tags such as ```<img />```,  ```<input />```, ```<audio>``` directly introduce content into the page. More on that later. 

### Closing vs. Self-closing tags

If the element contains other content, it ends with a closing tag.

For example:
```
<p>I contain content so I need to have a closing tag.</p>
```

Elements which do not contain content, like images, are self-closing. They do not required a closing tag.

```
<img src="image.jpg" />
```

Browsers interpret HTML elements to display a webpage.
