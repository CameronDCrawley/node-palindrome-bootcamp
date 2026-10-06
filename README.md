# ↔️ Week08 Bootcamp2019a Project: Server Side Palindrome Checker

### Goal: Create a simple web application that uses the fs and http modules to validate if a string is a palindrome server side.

### How to submit your code for review:

- Fork and clone this repo
- Create a new branch called answer
- Checkout answer branch
- Push to your fork
- Issue a pull request
- Your pull request description should contain the following:
  - (1 to 5 no 3) I completed the challenge
  - (1 to 5 no 3) I feel good about my code
  - Anything specific on which you want feedback!

Example:
```
I completed the challenge: 5
I feel good about my code: 4
I'm not sure if my constructors are setup cleanly...
```
Palindrome Checker 

Type in a word or phrase and find out if it's a palindrome. 

What's a Palindrome?

A word or phrase that reads the same forwards and backwards. Like racecar, level, or A man, a plan, a canal: Panama. My checker ignores spaces, punctuation, and capital letters, so that last one actually counts.

How It Works

You type something in and hit the button. The front end sends your word to my server's /api route, the server checks it, and sends back the answer as JSON.

The check itself happens in 3 steps:

Clean it up. A regular expression (/[^A-Z0-9]/ig) strips out everything that isn't a letter or number, then .toLowerCase() makes it all lowercase.
Flip it. .split('') breaks it into letters, .reverse() flips the order, and .join('') puts it back together.
Compare. If the cleaned-up word matches the flipped version, it's a palindrome.

Built With

- Node.js 
- JavaScript 
- HTML 
- CSS

  <img width="2880" height="1800" alt="image" src="https://github.com/user-attachments/assets/df1c1526-0e78-4923-b906-9ea7e9f0883b" />

