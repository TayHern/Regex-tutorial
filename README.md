# How to Use and Understand Regex

What is regex?  Many people new to web development like myself would be confused by this term.  Regex stands for regular expression.  Regular expression is used to define a specific search pattern by using sequences of characters.  So this can be used to match URLs, usernames, and passwords.  These algorithms or expressions within code can be used to find patterns of characters within strings, or to replace that sequence of characters by finding the pattern as well.

## Summary

There are many ways regex can be used in your own lines of code.  In this tutorial, we will be matching an email.  By doing this we are making sure that the user input is a valid email rather than just a bunch of words.  Below is line of regex code we will be using:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

Anchors have a special meaning in regex expressions.  These “characters” as you would know them from a non-technical or web development mind set, are not normal characters and do not match any characters to be used.  Instead they are used to match positions within the expressions.  
The caret or “^” stands for the beginning of the text or expression.
The dollar sign or “$” is used to represent the end of the text or expression.
So as you can see in our code snippet from above, the caret and the dollar sign represent the beginning and end of our expression:
/<b>^</b>([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})<b>$</b>/

### Quantifiers

Quantifiers match a number of occurrences of characters, groups, or character classes in strings.  In our code snippet, we use the + to signal that there will be another sequence.  As well, there is the {2,6} which signals that there must be a minimum of 2 characters and a max of 6.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Character Classes

Character classes represents character sets.  This meaning that it allows you to match any symbols with a certain character set.  You can do this by digits, word characters, or even white spaces.  In our code snippet, there one class currently.  
The \d in the code represents digits which are from 0-9.

### Grouping and Capturing

The capturing and grouping of sets show the sets of smaller expressions within the main regex expression.
There is the first set which represents the first part of the email of [a-z0-9_\.-]
The second set represents the domain of the email (e.g. google, yahoo) [\da-z\.-]
The third represents the domain extension (e.g. .com, .net) ([a-z\.]{2,6})

### Bracket Expressions

Bracket expression is a matching list or a non-matching list.  It usually consists of one or more expressions.
The first bracket expression includes case sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens. [a-z0-9_.-]
The second bracket expression includes all digits, case sensitive characters from a-z, periods and hyphens [\da-z.-]
The third bracket expression includes case sensitive characters from a-z and periods. [a-z\.]

### Greedy and Lazy Match

Greedy and Lazy match are more specific ways of identifying quantifiers.  Quantifiers are always by default greedy which means that they try to match as many as possible.  They also return the largest matches.  Lazy quantifiers are also known as non-greedy and match the preceding elements with the smallest matches by using a few of possible.  You can easily change from greedy to non-greedy by adding an extra ? to the expressions.  In our code snippet, we only use greedy quantifiers currently.  
In our code, the + matches the preceding element one or more times.
The brackets {} in our code match the preceding element from a certain amount of times, specifically 2-6 times.

## Author

Hi! I'm TayHern and I am an aspiring FullStack Developer with a growing knowledge of the coding world.  You can find me and my other work at: https://github.com/TayHern
