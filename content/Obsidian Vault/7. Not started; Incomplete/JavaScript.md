2024-07-3120:08
Status: #CS50 

JavaScript is a language built off of C that is run on the client’s side. Just like CSS with`<style>`tags, you can directly write your JavaScript between `<scrip>` tags. You can also write JavaScript in separate files and link them in by using the `scr` attribute of the `<script>` tag . JavaScript can behave like an object oriented language, where an object is similar to a structure in C. Where elements of the structure are called fields, members or properties. There are also methods which operate like functions that only operate on the object it is manipulating. `[object.function();]`

*Getbootstrap is a library that allows for easy formatting in HTML, CSS and JavaScript

Variables in JavaScript are similar to Python, the only difference is a need to distinct the variable with the var keyword.

Loops and If statements are identical in JavaScript to C

Additional loops in JavaScript:
```jsx
//Redux loop = itterate an operation across an array of data
for //(var key in object) 
{
	//use object[key] in here 
}
//or 
for //(var key of object) 
{
	// use key in here
}
```
```jsx
//Mapping methods onto objects operates across the entire array
var nums = [1,2,3,4,5];
nums = nums.map(function(num) {
	return num * 2; 
});
$2,4,6,8,10
```
All functions are introduced with the function keyword. JavaScript functions, particularly those bound specifically HTML elements can be anonymous (you don’t have to assign a name)

Array declaration: vars nums = `[1,2,3]`; *you can also have different variable types, vars mixed = `[true,’two’, 3]`

Events are a response to user interaction with a webpage

[https://www.example.com/path?key=value](https://www.example.com/path?key=value)

Common events that can be listened for: [blur][change][click][drag][focus][keyup][load][mousedown][mouseover][mouseup][submit][touchmove][unload]

DOC (Document Object Model) is an object in JavaScript that nests all the objects and data within a website into one object. Its structure is similar to that of tries in C.

```jsx
//Common DOM properties
innerHTML //Holds the HTML inside a set of HTML tags 
nodeName // The name of an HTML element or element's attribute 
id // The 'id' attribute of an HTML element 
parentNode // A reference to the node one level up in the DOM 
childNode //An array of references to the nodes one level down in the DOM 
attributes //An array of attributes of an HTML element 
style //An object encapsulating the CSS/HTML styling of an element  

//Common DOM Methods
getElementById(id) // Gets the elemenet with a given ID below this point in the DOM //'Id' in method is case sensitive 
getElementsByTagName(tag) // Gets all elements with the given tag below this point in the DOM
appendChild(node) //Add the given node to the DOM below this point
removeChild(node) //inverse of appendChild(node) 
```

Because the names of the objects can be quite long, the library, ‘jQuery’ is added. One thing it does is it simplifies DOM manipulations

[https://api.jquery.com](https://api.jquery.com)

```jsx
document.getElementById('colorDiv').style.backgroundColor = 'green' 
//Using the jQuery library it can also be written as
$('#colorDiv).css('background-color','green');
```