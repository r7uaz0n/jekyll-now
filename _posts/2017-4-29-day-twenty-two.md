---
layout: post
title: 4.29.2017 - Day Twenty-two - 
---

This is my twenty-second blog post made with Jekyll! Woohoo! 

## Today I learned (#TIL):   

- `parseInt()` function parses a string argument and returns an integer of the specified radix (the base in mathematical numeral systems).
_Syntax_
> parseInt(string, radix);

source:  [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt)

- socket.io  // interesting to learn more about this.

- package.json // the top level description of project, list of libraries that are being used (dependencies)

- Terminal - 
    * git clone - download a git
    * git branch - gives list of branches the project is using. (* which branch you are in)
    * git checkout - to switch to a different branch
    * -b to create a new branch
    * git status - tells which branch you are in

- start server in Terminal
    * node app.js
- close server in Terminal
    * ctrl c 

- Web browser web address:  localhost:8000

_socket.io flowchart from class_
![socketio_flowchart](/images/socketio_flowchart.jpg)

Breakdown of the JavaScript Event Listener
```javascript
    document.addEventListener('click', myFunction);
    function myFunction(event) {
        console.log(event);
}
```
VS

Breakdown of the SocketIO Event Listener
```javascript
        socket.on('my event', myFunction);
    function myFunction(data) {

        console.log(data);
}
```



_CALL BACK FUNCTIONS_

Breakdown of the JavaScript Event Listener
```javascript
    document.addEventListener('click', myFunction);
    function myFunction(event) {
        console.log(event);
}
```

SAME AS

Anonymous functions work too
```javascript
    document.addEventListener('click', function(event) {
        console.log(event);
});
```



Breakdown of the SocketIO Event Emitter
```javascript
socket.emit('my event', myData);
```

## Questions:


## Bugs discovered / what I got stuck on:

- Liz helped me dubug my 2D Breakout game code so I can continue working on it.  

## Useful links to save for later:

[xebra.js](https://cycling74.github.io/xebra.js/) - hope to explore this as I get more familiar with Javascript syntax


## My next goals:

- finish 2D Breakout game
- review socket.io class project
- catch up on past h/w and other stuff
- Just picked up this book.  [Make:  Getting Started with p5.js](https://p5js.org/books/)
I am thinking of documenting the results of the tutorial exercises here just for the sake of practice even though the tutorials might be pretty basic.  


# Perseverance is key!







