---
layout: post
title: 5.8.2017 - Monday - 
---

This is my twenty-sixth blog post:

## Today I learned (#TIL):   

- Attended a JS workshop today on how to make image filters like Instagram using the [CamanJS library](http://camanjs.com/) which was pretty neat.  

![caman1](/images/camanJS.png)
![caman2](/images/camanJS2.png)

Here's the JS code I worked on today.  There are six buttons.  1 reverts back to the original image. The others apply filters and performs a crop.  The example page on the CamanJS website is much cooler with the use of sliders to control parameters.  This is pretty barebones. 

```javascript
function revertFilter() {
	Caman('#my-image', function () {
	    this.reset()
	  });
}

function applyCustomFilter1() {
	Caman('#my-image', function () {
	    this.brightness(0);
	    this.contrast(30);
	    this.noise(60);
	    this.sepia(60);
	    this.saturation(60);
	    this.hue(50);
	    this.render();
	  });
}

function applyCustomFilter2() {
	Caman('#my-image', function () {
	    this.brightness(30);
	    this.contrast(15);
	    this.noise(20);
	    this.sepia(30);
	    this.saturation(20);
	    this.hue(90);
	    this.render();
	  });
}
function applyPremadeFilter1() {
	Caman('#my-image', function () {
	    this['orangePeel']();
	    this.render();
	  });
}

function applyPremadeFilter2() {
	Caman('#my-image', function () {
	    this['lomo']();
	    this.render();
	  });
}

function applyCrop() {
	Caman("#my-image", function () {
		
		// width, height, x, y
		this.crop(400, 500, 0, 500);  
		
		// Still have to call render!
		this.render();  
		});
}
```

Need to figure out how to export or publish the image now, just like Instagram.  :)


## Questions:

Is it possible to export or publish the image using only JS?


## Bugs discovered / what I got stuck on:


## Useful links to save for later:

[CamanJS library](http://camanjs.com/) 

## My next goals:

- Continue to practice JS
- Catch up on past H/W assignments and problems to solve
- Review some math
- Explore some web audio


# Perseverance is key!







