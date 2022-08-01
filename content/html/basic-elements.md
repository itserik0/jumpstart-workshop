+++
title = "Basic Elements"
date = 2021-06-17T16:34:21-04:00
weight = 1
+++

### Headings

HTML headings are defined with the ```<h1>``` to ```<h6>``` tags.

The ```<h1>``` is the top-level heading. It acts as the title of your document and is used only once per page.

```<h2>``` through ```<h6>``` can be used as many times as necessary in your content.

Don't use headings to make text bigger or bolder. Only use headings when they make sense as a title for discrete sections of content. 

Nest headings in the proper order to make your content easy to scan, and accessible for people who use screen readers. 

```
<h1>This is the page title</h1>
<h2>This is the second heading</h2>
<h3>This is the third heading</h3>
<h4>This is the fourth heading</h4>
<h5>This is the fifth heading</h5>
<h6>This is the sixth heading</h6>
```

### Paragraphs

Paragraphs are defined with the ```<p>``` tag:

```
<p>This is a paragraph.</p>
<p>This is the next paragraph.</p>
```
Those ```<p>``` will be rendered like this:

This is a paragraph.

This is the next paragraph.

### Links

Links are defined with the ```<a>``` tag:

```
<a href="https://www.website.com/">Link to website.com</a>
```
That link will be rendered like this:

[Link to website.com](https://www.website.com/)

This tag uses **attributes**. Attributes tell the browser more about how to render a certain element.

For ```<a>``` elements, the ```href``` attribute tells the browser where the link should go.

Element can have dozens of different attributes, as defined by the World Wide Web Consortium (W3C). If you use an attribute that is not supported for a given element, it will have no effect.

### Lists
There are three different list elements. Think about what type of list you are making to determine which list element to use. For example, a list of steps to complete a task should use a numbered list.

#### Unordered list (bulleted)

```
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

- Item 1
- Item 2
- Item 3
  
#### Ordered list (numbered)
```
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
```

1. Item 1
1. Item 2
1. Item 3

#### Description list
```
<dl>
    <dt>Deciduous tree</dt>
    <dd>drops leaves in cold months</dd>
    <dt>Evergreen tree</dt>
    <dd>does not lose leaves</dd>
</dl> 
```

Deciduous tree
: drops leaves in cold months  

Evergreen tree
: does not lose leaves


#### Tables

You may have heard tables are bad(!). That's because developers, in the past, would use tables layout their content. Tables are not good for laying out content, however, tables are great for tabular data:

```
<table>
    <th>
        <td>Name</td>
        <td>Age</td>
        <td>Email</td>
    </th>
    <tr>
        <td>Betty Smith</td>
        <td>27</td>
        <td>bsmith@email.com</td>
    </tr>
    <tr>
        <td>Robby Smith</td>
        <td>25</td>
        <td>rsmith@email.com</td>
    </tr>
</table>
```

| Name        | Age           | Email  |
| ------------- |:-------------:| -----:|
| Betty Smith      | 27 | bsmith@email.com |
| Robby Smith      | 25      |   rsmith@email.com |

#### Comments

HTML comments are not displayed in the browser. Their purpose is to document your code. 

```
<!-- This is a comment -->
```

You can also comment out code if you need to save it for later.

```
<!-- <img src="christmas-photo.jpg" width="25px" alt="Mall Santa endures screaming child on his lap" /> -->
```
