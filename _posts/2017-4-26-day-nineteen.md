---
layout: post
title: 4.26.2017 - Day Nineteen - 
---

This is my nineteenth blog post made with Jekyll! Woohoo! 

## Today I learned (#TIL):   


- I decided to go back to a challenge that I coudn't figure out which I decided to skip a while back.  With the help of the freeCodeCamp chat room I was able to figure it out.  

>Instructions:
>Modify the function `checkObj` to test `myObj` for `checkProp`. If the property is found, return that property’s value. If not, return `"Not Found"`.

My return wasn't correct and I also was replacing the value of `checkProp` when I put `checkProp=myObj;`


_incorrect_
```javascript
// Setup
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {
  // Your Code Here
  checkProp=myObj;
if (myObj.hasOwnProperty(checkObj) === true){
   return myObj;
    } else { 
  return "Not Found";
    }
}
// Test your code by modifying these values
checkObj("gift");
```

_correct_

```javascript
// Setup
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {
  // Your Code Here
//  checkProp=myObj;
if (myObj.hasOwnProperty(checkProp) === true){
   return myObj[checkProp];
    } else { 
  return "Not Found";
    }
}

// Test your code by modifying these values
checkObj("gift");
```


- Continued to work on 2D breakout game but didn't finish.  I remember the 2D primitive shapes used in [Processing](https://processing.org/) when I did some intro tutorials that have a similar syntax to JavaScript.  Good to note how to place these shapes on canvas.

	*rect () - the first two values specify the coordinates of the top left corner of the rectangle on the canvas, while the second two specify the width and height of the rectangle.
	
	syntax
> void ctx.rect(x, y, width, height);
	> 
	
	* arc() - x and y coordinates of the arc's center
	
	syntax
> void ctx.arc(x, y, radius, startAngle, endAngle, anticlockwise);



## Questions:



## Bugs discovered / what I got stuck on:



## Useful links to save for later:



## My next goals:

- continue to work on 2D breakout game
- work on other freeCodeCamp JavaScript Basics challenges



# Perseverance is key!







