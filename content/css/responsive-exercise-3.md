+++
title = "Responsive - Exercise #3"
date = 2021-06-17T16:34:21-04:00
weight = 6
+++

## Applying Media Queries

Let's apply a media query to the ```<header>```. The goal here is to make the header elements (the logo and the nav) stack up when the screen is below 768px.

```
header{
    background: red;
    display: grid;
    grid-template-columns: 1fr 1fr;
}

@media screen and (max-width: 768px) {
    header{
        display: block;
    }
}
```

The way to test this is to make the browser window skinny. Some browsers do have a responsive mode. 

Now apply this on the ```<main>``` and ```<article>``` elements.