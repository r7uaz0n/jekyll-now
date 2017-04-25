---
layout: post
title: 4.24.2017 - Day Seventeen - 
---

This is my seventeenth blog post made with Jekyll! Woohoo! 

- Got the broken image link working from Day 11.  I removed the image file and then reuploaded to Git.  Appears to be displaying properly now.

- Looking in to [Arrays on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) as I was trying to solve the Nesting For Loop problem.
	* lead me to look in to `forEach` method:  
	>"The forEach() method executes a provided function once for each array element."

*Syntax*
```javascript
arr.forEach(function callback(currentValue, index, array) {
    //your iterator
}[, thisArg]);
```

```javascript
var a = ['Rick', 'Monday', 'awesome'];

a.forEach(function(element) {
    console.log(element);
});
```
outputs:
```javascript
Rick
Monday
awesome
```



## Questions:



## Bugs discovered / what I got stuck on:

** Nesting For Loops ** freeCodeCamp challenge
Example code:
```javascript
var arr = [
  [1,2], [3,4], [5,6]
];
for (var i=0; i < arr.length; i++) {
  for (var j=0; j < arr[i].length; j++) {
    console.log(arr[i][j]);
  }
}
```
>Instructions
>Modify function `multiplyAll` so that it multiplies the `product` variable by each number in the sub-arrays of `arr`
```javascript
function multiplyAll(arr) {
  var product = 1;
  // Only change code below this line
for (var i = 0; i < arr.length; i++){  // not sure, just modeled after example code
  for (var j = 0; j < arr[i].length; j++){  // not sure, just modeled after example code
    console.log(arr[i][j]);  // not sure, just modeled after example code
  }
}
  
  // Only change code above this line
  return product;
}

// Modify values below to test your code
multiplyAll([[1,2],[3,4],[5,6,7]]);
```
- Still stuck on Nesting For Loops challenge.  Will move on to something else and get back to it.   



## Useful links to save for later:

I'm intrigued by this: [Johnny-Five](http://johnny-five.io/) 

## My next goals:

- finish up freeCodeCamp JavaScript Basics challenges
- work on h/w



# Perseverance is key!







