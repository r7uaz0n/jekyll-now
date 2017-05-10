---
layout: post
title: 5.9.2017 - Tuesday - 
---

This is my twenty-seventh blog post:

## Today I learned (#TIL):   

- I decided to go back to a freeCodeCamp challenge I have been stuck on which involved multi-dimensional arrays.  I decided to take it slow and read more on [JS arrays on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).


## Web Audio

- Just started to go through [Web Audio School](https://mmckegg.github.io/web-audio-school/).  Was able to make my browser play some simple oscillator tones in repl.it

```javascript
// create web audio api context
var audioContext = new AudioContext() 

// create Oscillator node
var oscillator = audioContext.createOscillator()  

oscillator.start(audioContext.currentTime)
oscillator.stop(audioContext.currentTime + 2) // stop after 2 seconds
oscillator.connect(audioContext.destination)
oscillator.type = 'sine'  // 'sine', 'triangle', 'sawtooth', or  'square'.
oscillator.frequency.value = 440;   // value in hertz
```

You can adjust the length of the tone by changing the number value in:   
oscillator.stop(audioContext.currentTime + 2) 

You can change the value of the hertz:  oscillator.frequency.value = 440;  

You an also change the oscillator.type using either:
'sine', 'triangle', 'sawtooth', and 'square'.



## Useful links to save for later:

[JS arrays on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

[Web Audio School](https://mmckegg.github.io/web-audio-school/)

[OscillatorNode.type](https://developer.mozilla.org/en-US/docs/Web/API/OscillatorNode/type)

## My next goals:

- Do more web audio school tutorials
- Continue to practice JS
- Catch up on past H/W assignments and problems to solve
- Review some math


# Read-Search-Ask

# Perseverance is key!








