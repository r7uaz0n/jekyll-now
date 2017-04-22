---
layout: post
title: 4.21.2017 - Day Fourteen - 
---

This is my fourteenth blog post made with Jekyll! Woohoo! 

## Today I learned (#TIL):   

- Learned about [JSON (JavaScript Object Notation)](http://www.json.org/)

>JSON (JavaScript Object Notationis a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. It is based on a subset of the JavaScript Programming Language, Standard ECMA-262 3rd Edition - December 1999. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C-family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others. These properties make JSON an ideal data-interchange language.JSON is built on two structures:

>A collection of name/value pairs. In various languages, this is realized as an object, record, struct, dictionary, hash table, keyed list, or associative array.
An ordered list of values. In most languages, this is realized as an array, vector, list, or sequence.
These are universal data structures. Virtually all modern programming languages support them in one form or another. It makes sense that a data format that is interchangeable with programming languages also be based on these structures.

source:  http://www.json.org/


10 challenges left until I'm done with the freeCodeCamp Basic JavaScript tutorial.
- Good progress today.  Challenges on Objects took me some time.

> Objects hold data in a property, which has a key-value format. In the example above, "artist": "Daft Punk" is a property that has a key of "artist" and a value of "Daft Punk".

Was stuck on this challenge on Manipulating Complex Objects.  I had forgotten to put a ',' after first object and to wrap second object in {}

Note:  arrays need commas between the values, and second object needs to be wrapped in {}

```javascript
var myMusic =  [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [ 
      "CS", 
      "8T", 
      "LP" ],
    "gold": true
  },
  {  
	"artist":"The Books",
    "title" : "The Lemon of Pink",
    "release_year": 2004,
    "formats": [
      "CD",
      "LP",
      "Data"],// Add record here
  }
];
```

- Worked on Week 2 H/W today:

# split()
> The `split()` method splits a String object into an array of strings by separating the string into substrings.

Syntax
str.split([separator[, limit]])


Source:  [MDN - String.prototype.split()()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)

**Example 1**
```javascript
var numb = "543210";
var answer = numb.split("");
console.log(answer);
```
outputs:  ["5", "4", "3", "2", "1", "0"]


**Example 2 - Removes spaces from `string`**
```javascript
var weekdays = 'Monday ;Tuesday; Wednesday ; Thursday ;Friday ';

console.log(weekdays);

var re = /\s*;\s*/;
var weekdaysList = weekdays.split(re);

console.log(weekdaysList);
```
outputs:  ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday "]


**Example 3 - Returns a limited number of splits**
```javascript
var myString = 'It is fun to learn JavaScript!';
var splits = myString.split(' ', 4);

console.log(splits);
```
outputs:  [It", "is", "fun", "to"]


**Example 4 - Capturing parentheses**
If separator contains capturing parentheses, matched results are returned in the array.
```javascript
var myString = 'Rick 1 learning. He 2 learning JS.';
var splits = myString.split(/(\d)/);

console.log(splits);
```
outputs:  ["Rick ", "1", " learning. He ", "2", " learning JS."]


**Example 5 - Reversing a String using split()**
```javascript
var str = '.kciR si eman yM';
var strReverse = str.split('').reverse().join(''); 
console.log(strReverse);
```
outputs:  My name is Rick.


## Questions:



## Bugs discovered / what I got stuck on:



## Useful links to save for later:

[JSON (JavaScript Object Notation)](http://www.json.org/) 

## My next goals:


# Perseverance is key!







