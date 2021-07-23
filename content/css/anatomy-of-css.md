+++
title = "Anatomy of CSS"
date = 2021-06-17T16:34:21-04:00
weight = 1
+++

## Anatomy of CSS

### CSS Ruleset

![CSS anatomy](../images/ruleset.png)

To modify multiple property values in one ruleset, write them separated by semicolons, like this:

```
p {
  color: red;
  width: 500px;
  border: 1px solid black;
}
```

### Multiple elements

To select multiple elements with one ruleset

```
h1, p, a {
  color: red;
}
```

### Types of Selectors

#### Element selector

All HTML elements of the specified type.

```
p {
    color: red;
}

h2 {
    color: blue;
}
```

#### ID Selector

The element on the page with the specified ID. On any HTML page id's need to be unique.

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

The element(s) on the page with the specified class. Use as many instances of the class name as you need.

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