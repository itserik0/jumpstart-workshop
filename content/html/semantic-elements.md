+++
title = "Semantic Elements"
date = 2021-06-17T16:34:21-04:00
weight = 2
+++

## What are Semantic Elements?

Semantic elements clearly describe their meaning to the browser and the developer.

Non-semantic elements like: ```<div>``` and ```<span>``` - tell nothing about its content.

Additionally, tags such as ```<b>``` (bold) and ```<i>``` (italics) define how the text should look, but don't provide any additional meaning to the markup. 

Semantic elements like: ```<form>```, ```<table>```, and ```<article>``` clearly define its content.


## Why Should We Use Semantice Elements?

The goal of any website its to communicate information. Aside from the page content, semantic markup gives us an additional opportunity to communicate meaning. 

Sites that rely on HTML code like: 

```
<div id="nav"> 
<div class="header"> 
<div id="footer">
```

to indicate navigation, header, and footer may help the developer but they don't help the browser understand what they are.

In these case it's more helpful to use:

```
<nav>
<header>
<footer>
```

Screen readers ignore visual styles and layout added using CSS. Semantic markup can aid screen readers in communicating the structure of the web page to its users.

Semantic markup can also be helpful to search engines, ensuring that the right pages are delivered for the right queries. 
 
## Semantic Elements

There are more than 100 semantic elements so we'll just look at the commonly used tags we haven't already touched on:

```
<article>
<aside>
<details>
<figcaption>
<figure>
<footer>
<header>
<main>
<mark>
<nav>
<section>
<summary>
<time>
```

### Section

The ```<section>``` HTML element represents a generic standalone section of a document, which doesn't have a more specific semantic element to represent it. Sections should have at least one heading.

```
<section>
    <h2>Latest News</h2>
    <p>News Story 1</p>
    ...
</section>

<section>
    <h2>Upcoming Events</h2>
    <p>Event 1</p>
    ...
</section> 
```

### Article

The ```<article>``` element specifies independent, self-contained content.

An article should make sense on its own, and it should be possible to distribute it independently from the rest of the web site.

```
<article>
    <h2>Wonder Bread Turns 100</h2>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit....</p>
</article>
```

## Nav

The ```<nav>``` element defines a set of navigation links. This tag is intended only for major blocks of links

```
<nav>
    <a href="/">Home</a> |
    <a href="/about">About</a> |
    <a href="/products">Products</a> |
    <a href="/contact">Contact</a> |
    <a href="/store">Store</a> |
</nav> 
```

#### Section vs Article

No hard rule here. You can have a ```<section>``` inside an ```<article>``` and an ```<article>``` inside a ```<section>```

### Header

The ```<header>``` element represents a container for introductory content or a set of navigational links.

```
<header>
    <img src="logo.jpg" />
    <nav>
        ...nav items
</header>
```

### Footer&nbsp;

The ```<footer>``` element defines a footer for a document or section.

```
<footer>
    <p>Copyright 2021: By Company Inc. All Rights Reserved.</p>
    <nav>
        <a href="/privacy">Privacy Policy</a>
        <a href="/contact">Contact Us</a>
        <a href="/location">Our Location</a>
</footer> 
```

You can have several ```<footer>``` elements in one document.

## Aside

The ```<aside>``` element defines some content aside from the content it is placed in (like a sidebar).

The ```<aside>``` content should be indirectly related to the surrounding content.

```
<section>
    <article>
        <h2>Article About Something</h2>
        <p>...</p>
    </article>
    <aside>
        <h2>Other Articles From This Week</h2>
        <h3>Article About This</h3>
        <h3>Article About That</h3>
    </aside>
</section>
```

## Figure 

The ```<figure>``` tag specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.

The ```<figcaption>``` tag defines a caption for a ```<figure>``` element. The ```<figcaption>``` element can be placed as the first or as the last child of a ```<figure>``` element.

The ```<img>``` element defines the actual image/illustration. 

```
 <figure>
  <img src="zebra_swallowtail_butterfly.jpg" alt="The black and white Zebra Swallowtail butterfly on a poppy flower.">
  <figcaption>Fig1. - Zebra swallowtail (Eurytides marcellus)</figcaption>
</figure> 
```