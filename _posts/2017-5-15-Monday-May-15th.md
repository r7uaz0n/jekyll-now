---
layout: post
title: 5.15.2017 - Monday - 
---

This is my thirtieth blog post: 


## Today I learned (#TIL):   

- Worked on some Codecademy tutorials for review and to gain some perspective to help me with _Loop Warmup HW_.  I haven't gone very far using Codecademy as I have been working more on freeCodeCamp so I last left off at if/else statements and logical/comparison operators.  Unlike freeCodeCamp, in Codecademy you are unable to skip ahead in the tutorials.  
`<switch>` hasn't come up in any projects or challenges we've worked on during the course so it was a nice refresh.  

```javascript
    var moonPhase = 'full';

    switch (moonPhase) {
     case 'full':
      console.log('Howwwlll!!');
       break;
    case 'mostly full':
       console.log('Arms and legs are getting hairier');
       break;
     case 'mostly new':
              console.log('Back on two feet');
          break;
      default:
      console.log('Invalid moon phase');
      break;
     }
```

- Solved last night's problem I got stuck on with help from Slack.  Revisited the use of `<continue>` .  

```javascript
  
    var i = 0;
    while (i < 5) {
     i++;
     if (i === 3) {
         continue;
     }
     console.log(i);
}
```

- Continued working on _Loop Warmup HW_.  



## Bugs discovered / what I got stuck on:

- Got stuck on this problem from the _Loop Warmup HW_:

>// CHALLENGE 17:
>// Write a WHILE loop that displays the numbers 1 to 20 (inclusive),
>// EXCEPT for numbers from 5 to 10 (inclusive) and from 15 to 19 (also inclusive).
>/* So your console should look like this:
>
>1 

>2

>3

>4 

>11

>12 

>13

>14

>20

Got more hints from Slack.  Here's some code I've been playing with but something is wrong with the logic:

```javascript
    var i = 0;
    while (i < 20) {
        i++;
        if ((i >= 5 || i <= 10) && (i >= 15 || i <= 19)) {
         continue;
     }
     console.log(i);
    }
```

Figured it out with more tinkering:

```javascript
  var i = 0;
  while (i < 20) {
      i++;
      if ((i >= 5 && i <= 10) || (i >= 15 && i <= 19)) {
          continue;
      }
      console.log(i);
  }
```

## My next goals:

- Finish _Loop Warmup HW_
- Continue to practice JS.  
- Catchup on past HW.

# Read-Search-Ask

# Perseverance is key!







