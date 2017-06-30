---
layout: post
title: 6.29.2017 - Thursday - 
---

This is my fiftieth blog post: 

## Today I learned (#TIL):   

- Attended GDI mentorship night and asked for help with the fCC challenge I was stuck on.  Solution below.

Challenge:
We have an array of objects representing different people in our contacts lists.

A ```lookUpProfile``` function that takes ```firstName``` and a property (```prop```) as arguments has been pre-written for you.

The function should check if ```firstName``` is an actual contact's ```firstName``` and the given property (```prop```) is a property of that contact.

If both are true, then return the "value" of that property.

If ```firstName``` does not correspond to any contacts then return ```"No such contact"```

If ```prop``` does not correspond to any valid properties then return ```"No such property"```

Solution:

```
javascript
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


function lookUpProfile(firstName, prop){
// Only change code below this line

for (var i = 0; i<contacts.length; i++)  {
  var contact = contacts[i];
  
  if (contact.firstName === firstName){
    if (contact[prop]!== undefined){
      return contact[prop];
    }
    else
      return "No such property";
  }
}
return "No such contact" ; 
// Only change code above this line
}

// Change these values to test your function
lookUpProfile("Akira", "likes");
```

- Now need to get back to working on the Firebase issues.


## Useful links:

[thimble](https://thimble.mozilla.org/en-US/) - an online code editor that makes it easy to create and publish your own web pages while learning HTML, CSS & JavaScript.


## My next goals:

- Continue to work on  _up for grabs_ issues. 
- Watch next section of Watch and Code JS video tutorials for review.

# Read-Search-Ask

# Perseverance is key!







