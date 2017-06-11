---
layout: post
title: 6.10.2017 - Saturday - 
---

This is my forty-first blog post: 

## Today I learned (#TIL):   

- Unforntunately, I didn't get to much blogging this week though I did get started on assigned HW challenges setting up Firebase in Git.  I had a cousin passing through I needed to attend to.  

- Sick today and unable to make it to class.  Worked remotely and finished working through HW 1 & 2 challenges and also received nice updates on Slack about what was happening in class today. Learned how to create and setup Firebase app and practiced displaying Firebase data on a webpage.  I hope I didn't miss out on too much from not being in class.  I find in-class time to be always valuable and it's always nice to see everyone in person as well.  Wish I had been present for the For Loop review but it was interesting working remotely.Looking forward to working with a mentor next week.

- I feel like I'm lacking on JS fluency by not actively practice coding in JS so I'm constantly relearning and going over things again. Having a project to work on is helpful.  

- Nice review on JS event listeners.

## Questions:

- When I commit something in GitHub, is it necessary to do all three steps of git add, commit and push in command line?

- What are some other practical purposes of using a database such as Firebase?


## Bugs discovered / what I got stuck on:

- Made a mistake placing the console.log outside of the body of the event.

incorrect:

```
	dbGreeting.on("value", function(dataSnapshot) {
   	 messageBox.textContent = dataSnapshot.val();
   	 });
	console.log( dataSnapshot.val() );
```

correct:

```
	dbGreeting.on("value", function(dataSnapshot) {
   	 messageBox.textContent = dataSnapshot.val();
   	 console.log( dataSnapshot.val() );
	});
```


## Useful links to save for later:

[Firebase JS reference](https://firebase.google.com/docs/reference/js/)

[JS Event reference](https://developer.mozilla.org/en-US/docs/Web/Events)

[Authenticate Using GitHub with JS](https://firebase.google.com/docs/auth/web/github-auth)


## My next goals:

- Continue working through HW challenges
- Continue to practice and review JS through Watch and Code videos.


# Read-Search-Ask

# Perseverance is key!







