**Palindrome Checker**

Type in a word or phrase and find out if it's a palindrome.

**What's a Palindrome?**

A word or phrase that reads the same forwards and backwards. Like **racecar**, **level**, or **A man, a plan, a canal: Panama**. My checker ignores spaces, punctuation, and capital letters, so that last one actually counts.

** How It Works **

You type something in and hit the button. The front end sends your word to my server's `/api` route, the server checks it, and sends back the answer as JSON.

The check itself happens in 3 steps:

1. **Clean it up.** A regular expression (`/[^A-Z0-9]/ig`) strips out everything that isn't a letter or number, then `.toLowerCase()` makes it all lowercase.
2. **Flip it.** `.split('')` breaks it into letters, `.reverse()` flips the order, and `.join('')` puts it back together.
3. **Compare.** If the cleaned-up word matches the flipped version, it's a palindrome.

** Built With **

- Node.js
- JavaScript
- HTML
- CSS

<img width="2880" height="1800" alt="Palindrome Checker screenshot" src="https://github.com/user-attachments/assets/df1c1526-0e78-4923-b906-9ea7e9f0883b" />

