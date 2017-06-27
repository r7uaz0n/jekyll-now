---
layout: post
title: 6.24.2017 - Saturday - 
---

This is my forty-eighth blog post: 

## Today I learned (#TIL):   

- I forgot to post this over the weekend. 

- Continued working through _Add Login with GitHub feature using Firebase Authentication_ issue.  Going through the steps is taking longer than I anticipated.  I got stuck on step 5 for some time where jshint.com suggesting I had an unmatched bracket.  Need to be more aware and careful of functions within functions. 

Incorrect code:

```
// When user clicks login button:
loginButton.addEventListener("click", function() {
// Use Firebase with GitHub Auth to log in the user
firebase.auth().signInWithRedirect(provider).catch(function(error) {
  // Log any errors to the console
  console.log(error);
});


// When user clicks logout button:
logoutButton.addEventListener("click", function() {
// Use Firebase with GitHub Auth to log in the user
firebase.auth().signOut().catch(function(error) {
  // Log any errors to the console
  console.log(error);
});
```

Correct code:

```
// When user clicks login button:
loginButton.addEventListener("click", function() {
  console.log("User clicked LOGIN"); 
  
  
        // Use Firebase with GitHub Auth to log in the user
      firebase.auth().signInWithRedirect(provider).catch(function(error) {
       // Log any errors to the console
       console.log(error);
      });
  
});


// When user clicks logout button:
logoutButton.addEventListener("click", function() {
  console.log("User clicked LOGOUT");
  
  
      // Use Firebase with GitHub Auth to log in the user
      firebase.auth().signOut().catch(function(error) {
       // Log any errors to the console
        console.log(error);
      }); 
  
});
```

- Finished __Add Login with GitHub feature using Firebase Authentication_ issue.  Yay!

- Working on _Up for grabs: Create a sample Firebase app that adds penguins to the database! #55_.

- Learned about creating data models.

Example taken from class:

> Here's the example data model outline we reviewed as a group on Saturday June 24th:

* users
  * userId
  * email
  * name
  * photoURL
  * bio
  * languages
    * languageId: skillLevel
* languages
  * languageId
    * name
    * description

> And here's a photo of the whiteboard, showing the same data model above:
![datamodelWB](/images/datamodelWB.jpg)

> Example JSON-formatted code for the above data model, with ONE sample user (with a "userId" of "1") and TWO languages:

```
var testDatabase = {
  "users": {
    "1": {
      "email": "..",
      "name": "Dan",
      "photoURL": "....",
      "bio": "....",
      "languages": {
        "33": 3,
        "12": 1
      }
    }
  },
  "languages": {
    "33": {
      "name": "JavaScript",
      "desc": "The scripting language of the web!"
    },
    "45": {
      "name": "HTML",
      "desc": "A markup language for structuring a web page."
    }
  }
};
```

- Use when testing Firebase database:
http://localhost:8080/

Links:

[JS	Hint](http://jshint.com/) - A Static Code Analysis Tool for JavaScript


## My next goals:

- Continue to work on  _up for grabs_ issues. 
- Watch next section of Watch and Code JS video tutorials for review.

# Read-Search-Ask

# Perseverance is key!







