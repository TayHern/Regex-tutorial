# How to Use and Understand Regex

What is regex?  Many people new to web development like myself would be confused by this term.  Regex stands for regular expression.  Regular expression is used to define a specific search pattern by using sequences of characters.  So this can be used to match URLs, usernames, and passwords.  These algorithms or expressions within code can be used to find patterns of characters within strings, or to replace that sequence of characters by finding the pattern as well.

For the full text on gist head to: https://gist.github.com/TayHern/cf7a8481860a3e24a7167b8b1556753b

## Summary

There are many ways regex can be used in your own lines of code.  In this tutorial, we will be matching an email.  By doing this we are making sure that the user input is a valid email rather than just a bunch of words.  Below is line of regex code we will be using:<br>
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Author

Hi! I'm TayHern and I am an aspiring FullStack Developer with a growing knowledge of the coding world.  You can find me and my other work at: https://github.com/TayHern
