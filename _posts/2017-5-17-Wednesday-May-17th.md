---
layout: post
title: 5.17.2017 - Wednesday - 
---

This is my thirty-second blog post: 


## Today I learned (#TIL):   

- Working on this problem from _Loop Warmup HW_ :

>CHALLENGE 20:
>Now combine the last two rules and write a WHILE loop that displays 1 to 10,
>EXCEPT for any multiple of 3 display the word "fizz" instead of the number,
>AND except for any multiple of 5, display the word "buzz" instead of the number!
>So your console should look like this:
>
>1 

>2

>fizz

>4

>buzz

>fizz

>7 

>8

>fizz

>buzz

Working this code but something is wrong:

```javascript
  var i=0;
  while (i<=9) {
    i++;
      var j = i % 3; 
        if (j === 0){
      console.log("fizz");
    } 
      var x = i % 5; 
        if (x === 0){
      console.log("buzz");
    }
    else{
    console.log(i);
  }
  }
```

It's logging the multiples of 3.  This is what the <console.log> outputs:

``` 
  1
  2
  fizz
  3
  4
  buzz
  fizz
  6
  7
  8
  fizz
  9
```
Was getting some hints from a couple of the coders on Slack but wasn't able to figure it out.  I had to step away and have some dinner before betting back to it. 



## What I got stuck on:

- Still stuck on the above problem.  Had a quick go using Python Tutor to track down the problem.  


## Useful links to save for later:

- After attending last night's Computer Vision meetup, out of curiousity I Google searched computer vision and JS. Came across [tracking.js](https://trackingjs.com/) - computer vision on the web.  

- [Python Tutor](http://www.pythontutor.com/)

## My next goals:

- Finish up _Loop Warmup HW_
- Review some math

# Read-Search-Ask

# Perseverance is key!







