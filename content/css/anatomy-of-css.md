+++
title = "Anatomy of CSS"
date = 2021-06-17T16:34:21-04:00
weight = 1
+++

## Anatomy of CSS

### CSS Ruleset

A CSS ruleset is comprised of a **selector**, which tell the browser which HTML elements to target, and **declarations**, which tell the browser what values to set for certain **properties** of the selected HTML element.

![CSS anatomy](../images/ruleset.png)

Declarations are separated by semicolons, like this:

```
p {
  color: red;
  width: 500px;
  border: 1px solid black;
}
```

### Multiple elements

To select multiple elements with one ruleset:

```
h1, p, a {
  color: red;
}
```

### Types of Selectors

#### Element selector

Select all HTML elements of the specified type.

```
p {
    color: red;
}

h2 {
    color: blue;
}
```

#### ID Selector

Select the element on the page with the specified ID. ```id``` is an attribute that can be applied to almost any HTML element, and must be unique. There should only be one of any given ```id``` on a webpage.

```
#my-id {
    width: 100px;
}
#my-other-id {
    width: 500px;
}
```

```
<div></div>
<div id="my-id"></div>
<div id="my-other-id"></div>
```

#### Class Selector

Select the element(s) on the page with the specified class. ```class``` is an attribute that, like ```id```, be applied to almost any element. However, unlike ```id```, multiple elements on the same webpage can have the same ```class```.

```
.my-class {
    font-weight: bold;
}
```

```
<ul>
    <li class="my-class">Dewey</li>
    <li class="my-class">Cheatum</li>
    <li class="my-class">Howe</li>
    <li>Smith</li>
</ul>
```

#### Descendent Selector

```
section .item{
    background-color: white;
}
```

#### Attribute selector

The element(s) on the page with the specified attribute.

```
a[href]{
    margin: 20px;
}
```

```
<a href="page.html">Link</a>
<a></a>
```

#### Pseudo-class selector

The specified element(s), but only when in the specified state. (For example, when a cursor hovers over a link.)

```
a:hover{
    text-decoration: underline;
}
```

#### Child Combinator

The child combinator (>) is placed between two CSS selectors. It matches only those elements matched by the second selector that are the direct children of elements matched by the first.

```
#things > p {
    margin: 2em;
}
```

```
<section id="things">
    <p>Apple</p>
    <p>Orange</p>
    <p>Banana</p>
    <div id="more-things">
        <p>Pineaplle</p>
        <p>Mango</p>
        <p>Blueberry</p>
    </div>
</section>
```

#### Adjascent Sibling

The adjacent sibling combinator (+) selects the element that immediately follows the first element, and both are children of the same parent element.

```
img + p {
  font-weight: bold;
}
```

```
<img src="image.jpg" />
<p>George Washington</p>
<p>John Adams</p>
```