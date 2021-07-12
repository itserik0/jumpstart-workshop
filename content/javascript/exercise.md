+++
title = "Basic Uses"
date = 2021-06-17T16:34:21-04:00
weight = 1
+++ 

## Selecting elements

There are 5 ways to select elements on an HTML page:

```
document.getElementsByTagName()
document.getElementsByClassName()
document.getElementById() *
document.querySelector()
document.querySelectorAll() *
```

## Manipulating text

```
<div id="example"></div>
```

```
document.getElementById("example").innerHTML = "Hello!";
```

```
<div id="example">Hello!</div>
```

## Change Styling

```
document.getElementById("example").style.fontSize = "25px";
document.getElementById("example").style.color = "red";
document.getElementById("example").style.backgroundColor = "yellow"; 
```

## Change Attributes

```
document.getElementById("example-image").src = "picture.gif";
```

or

```
document.getElementById("example").classList.add("my_class_name");
```

## Events and Interactivity

Events are things that happen in the browser — a button being clicked, a page loading, a video playing, etc. — in response to which we can run blocks of code.

To listen for these events we have to create an **event listener** and the blocks of code that run in response to the event firing are called **event handlers**.

```
<button id="my-button>click me</button>
```

```
document.getElementById("my-button").addEventListener("click", handle_button_click);

function handle_button_click(){
    //do some stuff
}
```

### Types of events

- Mouse events
  - mousedown, mouseup, click, dblclick, mousemove, mouseover, mousewheel, mouseout, contextmenu
- Touch events
  - touchstart, touchmove, touchend, touchcancel
- Keyboard events
  - keydown, keypress, keyup
- Form events
  - focus, blur, change, submit
- Window events
  - scroll, resize, hashchange, load, unload