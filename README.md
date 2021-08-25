# react_unorderlist
Created with CodeSandbox 
Notes from React module.     
The Complete 2021 Web Development Bootcamp     
Instructor: Dr. Angela Yu      

## Description
This project is an introduction to React,    
It displays a Heading and     
an unordered list (bullet points) with 3 items.     
These items are 3 animals I like: Wombat, Koala and Quokka.    

## How to use React
To be able to use React,      
We need to create, in our index.html file, a div with the id="root"     
```
<div id="root"></div>
```
This is the root of our React Application     
Everything created with React will be inserted in this div.

The script in our HTML file that links to our JS file, must be changed: type= from javascript to JSX, eg:      
```
<script src="../src/index.js" type="text/JSX"></script>
```

The HTML file won't be used anymore,     
all the code is written in the JS file using JS and React

In our JS file (index.js by convention):        
The first step will be to import React and ReactDom modules      
```
import React from "react";
import ReactDOM from "react-dom";
```
Now we can use both packages:      
ReactDom.render() takes 2 inputs:      
* Input 1: What to show
* Input 2: Where to show
* Input 3 (optional) : callback function whnt render is complieted  

Eg: [React Tutorial: Hello World](https://github.com/ChristianVillalba/react_tutorial.git)
```
ReactDOM.render(
  <h1>Hello World</h1>,
  document.getElementById('root')
 );

```
We placed an H1 Element (what) inside our div id="root" (where)      
React creates this as a JSX file, 
this way index.js knows that is HTML and not JS.

The ReactDom render method can take only ONE ELEMENT        
But we can put as many elements as we want into one single div element         
Eg: [React Tutorial: Unordered List](https://github.com/ChristianVillalba/react_unorderlist)
```
ReactDOM.render(
  <div>
    <h1>This is React!</h1>
    <ul>
      <li>Wombat</li>
      <li>Koala</li>
      <li>Quokka</li>
    </ul>
  </div>,
  document.getElementById("root")
);
```

## What I have learned with this project:
* Change our js script in HTML from type="text/javascrip" to type="text/JSX"
* Link and fork using codesandbox
* import "React" and "ReactDom"
* Using ReactDom to render elements
  * Using the inputs that the render method needs
  * Using a single div to render mulitiple HTML Elements 
