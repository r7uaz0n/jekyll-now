---
layout: post
title: 6.21.2017 - Wednesday - 
---

This is my forty-seventh blog post: 

## Today I learned (#TIL):   

- Day 13 of my cold and now about 95% recovered.  Still experiencing some chest congestion which is causing me to cough.  

- Worked on _Add Login with GitHub feature using Firebase Authentication_ issue.  Had to go back to review how to set up event listeners and get that working with a button.  Made JavaScript objects for the Login and Logout buttons and had them print to the console when pressed.

```
var loginButton = document.getElementById("loginbtn");
var logoutButton = document.getElementById("logoutbtn");

loginButton.addEventListener("click", function (event) {
  console.log("User clicked LOGIN");
});

logoutButton.addEventListener("click", function (event) {
  console.log("User clicked LOGOUT");
});
```

- Looking at the Solution code, I noticed I was missing the following line of code:

```
var userInfoBox = document.getElementById("userinfo");
```

I looked back at the issues and couldn't locate where I should have done this.  So I went ahead and just added to my firebasetest.js as well as added the appropriate HTML tags to my index.html file.


## My next goals:

- Continue to work on _Add Login with GitHub feature using Firebase Authentication_ issue.
- Look at _up for grabs_ issues and select something to work on. 
- Watch next section of Watch and Code JS video tutorials for review.

# Read-Search-Ask

# Perseverance is key!







