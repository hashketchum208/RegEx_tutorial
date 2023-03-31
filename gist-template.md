# RegEx_matchEmailTutorial

RegExr is an online tool to learn, build, & test Regular Expressions (RegEx / RegExp).

## Summary

In this section, I will demonstrate the use of regular expressions by using email matching

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

 Matching an Email: `/^([a-z0-9_\.-]+)@(([\da-z\.-]+)+)\.([a-z\.]{2,6})$/`,

### Anchors

Notice the ^ and $, these are our anchors. These will act as beginning and end points for the strings we want to match.

### Quantifiers

This is used to set limits of the number of characters that can be matched. They will most commonly be used for minimum and maximum matching. In our example, our quantifiers are {2,6}.

### Grouping Constructs

Grouping Constructs are a bit complicated to explain, as there is 2 different ways to aim what you want to match and capture. To follow protocol, you would use parentheses (()). We have the @ breaking the groups.

### Bracket Expressions

The [] brackets acts as a range of characters we want to match. In our case we have several of these arrays, one is just looking for 0-9 but is called as a character \d

### Character Classes

We already shed a bit of light on Character Classes earlier. Whe had \d looking for 0-9. How this really works is its looking for any Arabic numeral digit. There are many other character classes, like \s, which matches a single whitespace character, including tabs and line breaks.

### The OR Operator

When we see our first range of characters [a-z0-9_\.-] we see that its looking for all lower case characters and numbers between 0-9 OR four unique characters. Those characters being the characters following 0-9.

### Flags

Flags are used to wrap the slashes in our expression at the end to define additional functionality or limits for the regex. Six different flags are used but typically it will be:
g - Global search
i—Case-insensitive search
m—Multi-line search

### Character Escapes

A prime example of this in our example is after the grouping looking for the actual email webhost string. We see \. , this is showing us to just look for the . as its own character in the expression. meaning this . is found as 
.com. It is being held out of the brackets and strings alltogether.

## Author

Leo Pignanelli is the name, and breaking your code is the game. Please feel free to reach out to me if anything found here is incorrect or I am viewing in the wrong way. Keep watching the skies!!

https://github.com/hashketchum208