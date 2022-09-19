# Week 17 - Regex Tutorial

This weeks Project is a tutorial to explain what is and how to use and understand, a regular expression otherwise known as a Regex.

## Summary
This tutorial will be covering a Regex used for matching emails.
it is a fantastic tool to use in your code for retrieving information from a body of code and also for using as validation in your projects.
This tutorial will cover all the information you need to use and understand Regular Expression components.
<br>

* Matching an Email Regex: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
The anchors of a Regex is what is used to both start and finish the line of code you are trying to find.

Example: <br>
`/^`([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`$/`
<br>
in the line of code above highlighted the `/^` and `$/` as they are the start and end points for the entire Regex.

### Quantifiers
Quantifiers are symbols used to define how many times your chosen characters are required to be present in order to get a match or a successful validation.

Example: 
<br>
/^`([a-z0-9_\.-]+)`@`([\da-z\.-]+)`\.([a-z\.]{2,6})$/
<br>
In the above i have highlighted where the quantifier is being used. 
Where is shows `a-z0-9_\.-` it is stating that at least one of these are required before the @ symbol. ie = abc123@ would be a match.
<br>
The second group i highlighted `([\da-z\.-]+)` must also be matched using one or more digits, letters from a-z periods . and hyphens - <br> It then has to be followed by a period .

### Grouping Constructs
Example: /^`(`[a-z0-9_\.-]+`)`@`(`[\da-z\.-]+`)`\.`(`[a-z\.]{2,6}`)`$/
<br>
So with our Regex code the symbols used for grouping are the round brackets ( ),i have highlighted them above in the regex.
<br>
The characters in between the brackets need to be matched and meet the groups requirements before moving onto further steps of the regex.

### Bracket Expressions
These are used to the enclose the characters you wish to be matched in your code.
<br>
/^(`[`a-z0-9_\.-`]`+)@(`[`\da-z\.-`]`+)\.(`[`a-z\.`]`{2,6})$/
<br>
Example: if i wanted to an exact match for abcd i would use [abcd], or any of those characters would be [a-d] or if i wanted those letters excluded and allow all others except those i would use [^abcd] or [^a-d].

### Character Classes
/^([`a-z0-9_\.-`]+)@([`\da-z\.-`]+)\.([`a-z\.`]{2,6})$/
<br>
The character class, also known as the character set is a simple concept as they are just the chosen characters you are looking for when using the regex, whatever characters you put inside the square brackets become your character class or chracter set
<br>
Example: [`a-z0-9_\.-`]
<br>
Highlighted above is the chosen character class/ set for the regex
<br>

### The OR Operator

For our chosen Regex, we arent using an OR operator. but i will still explain what it is and how to use it.
<br>
The OR operator is the pipe or "vertical bar" symbol  which is: |
<br> 
Similiar to the double pipe symbols used in coding logic.
<br>
Example: [a-z|0-9]
<br>
In the example used above requires you to use letters a-z OR numbers 0-9. Another simple explanation would be [a|b] other wise spoken like "option (a) OR option (b)

### Character Escapes
/^([a-z0-9_`\`.-]+)@([`\`da-z`\`.-]+)`\`.([a-z`\`.]{2,6})$/
<br>
The above example has the escape symbol highlighted, it is the back slash \, it is used to escape special characters like periods, dashes etc

## Author

[GitHub Repo](https://github.com/JRoberts94/Week17-Regex-Tutorial/blob/main/Regex-Tutorial.MD)
<br>
[GitHub Profile](https://github.com/JRoberts94)