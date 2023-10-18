# Title Welcome to the rebranded regexRegus

We're taking markdown to a whole different level. When you think about your mark down needs, you have you covered with regexRegus.

## Summary

Have you ever been in a situation when you need some validation of the characters of Email? The regexRegus app will help you.
The regez line I will be defining will be Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
^: Anchor the match at the beginning of the string.
$: Anchor the match at the end of the string.


### Quantifiers
([a-z\.]{2,6}): This part captures the top-level domain (TLD), which can be 2 to 6 lowercase letters or periods. It consists of:

[a-z\.]{2,6}: A character class [...] that matches between 2 and 6 occurrences of lowercase letters or periods. This represents the allowed characters in the TLD.

### OR Operator
This line of regex does not have an OR Operator

### Character Classes
[a-z0-9_\.-]+: A character class [...] that matches one or more occurrences of lowercase letters, digits, underscores, periods, or hyphens. This represents the allowed characters in the local part.

([\da-z\.-]+): This part captures the domain name. It consists of:

[\da-z\.-]+: A character class [...] that matches one or more occurrences of digits (\d), lowercase letters, periods, or hyphens. This represents the allowed characters in the domain name.

[a-z\.]{2,6}: A character class [...] that matches between 2 and 6 occurrences of lowercase letters or periods. This represents the allowed characters in the TLD.


### Flags
This line of regex does not have any flags

### Grouping and Capturing
([a-z0-9_\.-]+): This part captures the local part of the email address (the part before the '@' symbol).
([\da-z\.-]+): This part captures the domain name
([a-z\.]{2,6}): This part captures the top-level domain (TLD), which can be 2 to 6 lowercase letters or periods

### Bracket Expressions
Anything that is in between square or curly brackets.

The first character class [a-z0-9_\.-] is used in the local part (before the '@' symbol) and allows letters, digits, underscores, periods, and hyphens.
The second character class [\da-z\.-] is also used in the local part and allows digits, lowercase letters, periods, and hyphens.
The third character class [a-z\.] is used in the top-level domain (TLD) and allows lowercase letters and periods.

### Greedy and Lazy Match
There are no greedy or lazy matches in this regex 

### Boundaries
There are no boundaries in this regex 

### Back-references
There are no back-references in this regex 

### Look-ahead and Look-behind
There are neither look-ahead nor look behind references in this regex

## Author
Gabriel Regus us a student at Columbia University School of Engineering, where he is completing a Coding Bootcamp.  

https://github.com/ColumbiaCoding/