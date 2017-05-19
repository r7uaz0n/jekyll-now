---
layout: post
title: 5.18.2017 - Thursday - 
---

This is my thirty-third blog post: 


## Today I learned (#TIL):   

- Attended _Mentorship night at Pivotal Labs_ which was fun.  It was a great opportunity to meet various people with different backgrounds working in tech to ask questions about their background experience, advice as well as help on some problems.   I'm glad I went and hope to attend again.  I will have more questions prepared for next time.  

- Was stuck on the same problem from yesterday but someone from tonight's meetup helped me out:

solution:

```javascript
  var i=0;
  while (i<10) {
    i++;
    var j = i % 3;
    var x = i % 5; 
    if (j === 0) {
      console.log("fizz");
    } else if (x === 0) { 
     console.log("buzz");
    } else {
     console.log(i);
    }
  }
```

I was also introduced to another way to solve the problem which I started at the Meetup and finished at home.  I'm wondering if setting `var i=1;` is correct.  Though it does solve the problem:

```javascript
  var i=1;
  while (i<=10) {
    var j = i % 3;  
    if (j === 0) {
      console.log("fizz");
    i++;
    }  
    var x = i % 5;  
    if (x === 0) { 
      console.log("buzz");
    i++;
    } else {
      console.log(i);
    i++;
    }
  }
```

The Challenge once again:

>CHALLENGE 20:
>Now combine the last two rules and write a WHILE loop that displays 1 to 10,
>EXCEPT for any multiple of 3 display the word "fizz" instead of the number,
>AND except for any multiple of 5, display the word "buzz" instead of the number!
>So your console should look like this:

Both sets of code above log the following:

```
  1
  2
  fizz
  4
  buzz
  fizz
  7
  8
  fizz
  buzz
```

I need to keep practicing.


## What I got stuck on:

- Working on final problem of _Loop Warmup HW_ :

>CHALLENGE 21:
>Now change the previous loop to display numbers from 1 to 15, and change it so that
>if a number is a multiple of BOTH 3 and 5, display "fizzbuzz".
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

>11

>fizz

>13

>14

>fizzbuzz 


Will continue on this one tomorrow.


## My next goals:

- Solve final H/W of _Loop Warmup HW_.
- Practice more JS

# Read-Search-Ask

# Perseverance is key!







