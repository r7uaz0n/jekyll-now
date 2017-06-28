---
layout: post
title: 6.27.2017 - Tuesday - 
---

This is my forty-ninth blog post: 

## Today I learned (#TIL):   

- Now that the (un)bootcamp is finished I need to make an effort to continue practicing JS.  Glad to still have a project to work on.  I decided to go back to some fCC problems.  I feel determined to finish the fCC JavaScript challenges.  

- Working on fCC [_Profile Lookup_ challenge](https://www.freecodecamp.com/challenges/profile-lookup) which I got stuck on:

Challenge:
We have an array of objects representing different people in our contacts lists.

A ```lookUpProfile``` function that takes ```firstName``` and a property (```prop```) as arguments has been pre-written for you.

The function should check if ```firstName``` is an actual contact's ```firstName``` and the given property (```prop```) is a property of that contact.

If both are true, then return the "value" of that property.

If ```firstName``` does not correspond to any contacts then return ```"No such contact"```

If ```prop``` does not correspond to any valid properties then return ```"No such property"```


Incorrect code:

```

//Setup
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["Javascript", "Gaming", "Foxes"]
    }
];

function lookUpProfile(firstName, prop) {
// Only change code below this line

for (var i=0; i<4; i++) {
  if (contacts[i].firstName !== firstName){
     return "No such contact";
  } else if (contacts[i].prop!== prop){
     return "No such property";
  } else { 
     return prop;
  }
}  

// Only change code above this line
}

// Change these values to test your function
lookUpProfile("Akira", "likes");
```


- Review
> For loops are declared with three optional expressions separated by semicolons:

```for ([initialization]; [condition]; [final-expression])```



## My next goals:

- Solve above challenge
- Continue to work on  _up for grabs_ issues. 
- Watch next section of Watch and Code JS video tutorials for review.

# Read-Search-Ask

# Perseverance is key!







