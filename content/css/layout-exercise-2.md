+++
title = "Layout - CSS Exercise #2"
date = 2021-06-17T16:34:21-04:00
weight = 4
+++

### Reset styles

Browsers come with default styles for some elements, and these defaults vary among browsers. The first thing many websites do is to add reset styles to remove them. Let's start with adding this to our styles:

```
*{
    padding: 20px;
}

html,body{
    padding: 0px;
    margin: 0px;
}
```

### Let's see what the layout looks like

Let's go back to the html page we made. Right now it probably looks like a confusing bunch of text. 

We can get a better idea of what the layout looks like using CSS. 

1. Open the **styles.css** file.
2. In your styles add a unique background color for each of the following elements: 
   - header
   - nav
   - main
   - article
   - section
   - aside 
   - footer
3. If your HTML is done correctly it should now look just as ugly as this:

![colorful layout](../images/Terrible_Recipes_1.png)

### The Grid

A typical web page layout is not elements stacked visually on top of each other. Elements go both horizontal and vertical.

![typcial layout](../images/layout.png)

In the bad old days of CSS there were many ways of doing this but they were all not great. You may have heard about stuff like **floats** or **display: inline-block**, or (fog horn sound) **absolutely positioning elements** (this is what build-your-own sites like Wix and Squarespace use). 

#### The grid 

![the grid](../images/grid.jpg)

When laying out elements we want to think them in terms of a grid like we have above. When the page is broken up into columns like the grid does than we can stretch elements across one or many columns. 

![typcial layout](../images/layout-with-grid.png)

Doing this in CSS is fairly simple. We apply these properties to the parent element:

```
display: grid;
grid-template-columns: 1fr 1fr;
```

So if this parent element has two element they will each be divided into 1 fr or fraction each. 

Let's work together to turn our existing HTML page into a grid layout.

#### The Header

```
header{
    background: red;
    display: grid;
    grid-template-columns: 1fr 1fr;
}
```

#### The Main area

```
main{
   background: orange;
   display: grid;
   grid-template-columns: 2fr 1fr;
}
```

#### The Article

```
article{
   background: green;
   display: grid;
   grid-template-columns: 1fr 1fr;
}
```