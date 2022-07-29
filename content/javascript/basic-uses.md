+++
title = "Exercise"
date = 2021-06-17T16:34:21-04:00
weight = 2
+++ 

## Let's have some fun

So far this workshop has been a lot of information. Now let's use Javascript to make our webpage interactive!

### An Alert

somewhere in index.html
```
<button id="my-button">click me</button>
```

in script.js
```
document.getElementById("my-button").addEventListener("click", handle_button_click);

function handle_button_click(){
    alert("I am an alert");
}
```

### Change text

somewhere in index.html
```
<p>Hello. My name is <span id="persons-name"></span>.</p>
<input type="text" id="my-input" value="" />
<button id="my-button">add my name</button>
```

in script.js
```
document.getElementById("my-button").addEventListener("click", handle_button_click);

function handle_button_click(){
    document.getElementById("persons-name").innerText = document.getElementById("my-input").value;
}
```

### Validate a form element

somewhere in index.html
```
<h2>Please enter a valid number</h2>
<input type="text" id="my-input" />
<button id="my-button">Submit number</button>
<span id="validation-message"></span>
```

```
document.getElementById("my-button").addEventListener("click", handle_button_click);

function handle_button_click(){
    var text_input = document.getElementById("my-input").value;
    if(isNaN(text_input) == true){
        document.getElementById("validation-message").innerText = "That ain't no number.";
    }else{
        document.getElementById("validation-message").innerText = "You have entered a valid number";
    }
}
```