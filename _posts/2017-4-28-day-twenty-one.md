---
layout: post
title: 4.28.2017 - Day Twenty-one - 
---


This is my twenty-first blog post made with Jekyll! Woohoo! 

## Today I learned (#TIL):   

- Watched a short [Max MSP: Intro to JavaScript](https://www.youtube.com/watch?v=0Yfqp2I_Chw) tutorial._  I haven't thought how I can use JS in Max yet as I've been focused more on learning JS.  There is an algorithm related to probability I may consider using JS.  I'll have to pick the brain of someone who is good with probability and algorithms.  
- Did some math exercises in Khan Academy.  Did some pre-algebra exercises.  Most were too easy though good to refresh and get warmed up to practice math again.
- Continued working on 2D Breakout game. 
Ugh oh, multi-dimensional arrays in lesson 6. 


## Questions:

- Something came up while doing 2D Breakout game about how things are ordered as the code in the tutorial did not match exactly the code I had based on the tutorial.  Does it matter in what order things are in code?  Should all `functions` be towards the top?  I think I answered that Q for myself.  See below. 


## Bugs discovered / what I got stuck on:

- I had followed the instructions in Lesson 5 and noticed my paddle controls were not working when I press the left and right arrow keys.  I then Compared my code with the code of the tutorial and moved things around so my code was identical to the code in the tutorial.  Paddle control started working.  The tutorial is a bit confusing because it misleads so that the code does not actually work in the order it instructs but differs from the code that is displayed in the _Compare your code_ section. 

_My code following the instructions_ Lesson 5 - (paddle doesn't work)

```javascript
<script>
// JavaScript code goes here
var canvas = document.getElementById("myCanvas"); 
var ctx = canvas.getContext("2d");  
var ballRadius = 10;
var x = canvas.width/2;
var y = canvas.height-30;
var dx = 2;
var dy = -2;
var paddleHeight = 10;
var paddleWidth = 75;
var paddleX = (canvas.width-paddleWidth)/2;
var rightPressed = false;
var leftPressed = false;

// drawing code
function drawball(){
	ctx.beginPath();
	ctx.arc(x, y, ballRadius, 0, Math.PI*2);
	ctx.fillStyle = "#0095DD";
	ctx.fill();
	ctx.closePath(); 
}

function draw() {  
	ctx.clearRect(0, 0, canvas.width, canvas.height);
	drawball();
    drawPaddle();

    if(x + dx > canvas.width-ballRadius || x + dx < ballRadius) {
    dx = -dx;
    }
    if(y + dy < ballRadius) {
    dy = -dy;
    } 
    else if(y + dy > canvas.height-ballRadius) {
        if(x > paddleX && x < paddleX + paddleWidth) {
            dy = -dy;
        }
        else {
            alert("GAME OVER!");
            document.location.reload();
        }
    }

	x += dx;
    y += dy;
    }

    if(rightPressed && paddleX < canvas.width-paddleWidth) {
        paddleX += 7;
    }
    else if(leftPressed && paddleX > 0) {
        paddleX -= 7;
    }

function drawPaddle() {
    ctx.beginPath();
    ctx.rect(paddleX, canvas.height-paddleHeight, paddleWidth, paddleHeight);
    ctx.fillStyle = "#0095DD";
    ctx.fill();
    ctx.closePath();
}


document.addEventListener("keydown", keyDownHandler, false);  // listens for keydown presses
document.addEventListener("keyup", keyUpHandler, false);  // listens for keyup presses

function keyDownHandler(e) {
    if(e.keyCode == 39) {
        rightPressed = true;
    }
    else if(e.keyCode == 37) {
        leftPressed = true;
    }
}
function keyUpHandler(e) {
    if(e.keyCode == 39) {
        rightPressed = false;
    }
    else if(e.keyCode == 37) {
        leftPressed = false;
    }
}

setInterval(draw, 10);
</script>
``` 

_Compare your code_ section Lesson 5 - (paddle works!)
```javascript
<script>
// JavaScript code goes here
var canvas = document.getElementById("myCanvas"); 
var ctx = canvas.getContext("2d");  
var ballRadius = 10;
var x = canvas.width/2;
var y = canvas.height-30;
var dx = 2;
var dy = -2;
var paddleHeight = 10;
var paddleWidth = 75;
var paddleX = (canvas.width-paddleWidth)/2;
var rightPressed = false;
var leftPressed = false;

document.addEventListener("keyup", keyUpHandler, false);  // listens for keyup presses
document.addEventListener("keydown", keyDownHandler, false);  // listens for keydown presses

function keyDownHandler(e) {
    if(e.keyCode == 39) {
        rightPressed = true;
    }
    else if(e.keyCode == 37) {
        leftPressed = true;
    }
}

function keyUpHandler(e) {
    if(e.keyCode == 39) {
        rightPressed = false;
    }
    else if(e.keyCode == 37) {
        leftPressed = false;
    }
}

// drawing code
function drawball(){
	ctx.beginPath();
	ctx.arc(x, y, ballRadius, 0, Math.PI*2);
	ctx.fillStyle = "#0095DD";
	ctx.fill();
	ctx.closePath(); 
}

function drawPaddle() {
    ctx.beginPath();
    ctx.rect(paddleX, canvas.height-paddleHeight, paddleWidth, paddleHeight);
    ctx.fillStyle = "#0095DD";
    ctx.fill();
    ctx.closePath();
}


function draw() {  
	ctx.clearRect(0, 0, canvas.width, canvas.height);
	drawball();
    drawPaddle();

    if(x + dx > canvas.width-ballRadius || x + dx < ballRadius) {
        dx = -dx;
    }
    if(y + dy < ballRadius) {
        dy = -dy;
    } 
    else if(y + dy > canvas.height-ballRadius) {
        if(x > paddleX && x < paddleX + paddleWidth) {
            dy = -dy;
        }
        else {
            alert("GAME OVER!");
            document.location.reload();
        }
    }

    if(rightPressed && paddleX < canvas.width-paddleWidth) {
        paddleX += 7;
    }
    else if(leftPressed && paddleX > 0) {
        paddleX -= 7;
    }

    x += dx;
    y += dy;
}

setInterval(draw, 10);
</script>
```

Just noticed this same problem in Lesson 7.  

## Useful links to save for later:

[MAX MSP: INTRODUCTION TO JAVASCRIPT PT1](https://www.youtube.com/watch?v=0Yfqp2I_Chw)

## My next goals:


# Perseverance is key!







