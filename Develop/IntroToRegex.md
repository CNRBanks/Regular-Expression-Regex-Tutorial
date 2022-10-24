# Intro to Regular Expressions

## Summary

This is a introduction on how to interpret regular expressions, commonly referred to as regex. For this tutorial we will look at a regex that was written to assist with searching text for email addresses.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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

The email address regex has two anchors - " ^ " and " $ " - located at the beginning and end of the expression.

The carrot anchor (^) denotes a string that begins with the characters that follow it. In this instance the characters that follow the anchor are `([a-z0-9_\.-]+)`.

The dollar anchor ($) denotes a string that ends with the characters that precede it. In this instance the characters that precede the anchor are `@([\da-z\.-]+)\.([a-z\.]{2,6})`.

### Quantifiers

Quantifiers determine the limit of the string that the regex matches. Quanitifiers commonly include the minimum and maximum number of characters that the regex is searching for.
Our given email address regex has the following quantifier -

`{2,6}` - This signifies that the regex will match the preceding characters a minimum of 2 times to a maximum of 6 times. Any pattern of characters that appears in the text less than twice or more than six times will not be captured by this regex.

### OR Operator

### Character Classes

In a regular expression the character classes define a set of characters, any one of which can be used in an input string to locate a match. One character class used in the provided email address regex is " \d " which matches any numeric digit, and is essentially the equivalent of [0-9].


### Flags

### Grouping and Capturing

### Bracket Expressions

The email address regex contains a number of bracket expressions. Bracket expressions are defined as a anything inside a set of square brackets ([]), and they represent a range of characters that the user wants to search for.

[a-z0-9_\.-] - Any characters from a to z (only lowercase), any number from zero to nine, as well as the symbols " _ ", " . " and " - ".
[\da-z\.-] - The "d" is searching for any digit, any character from a to z, as well as " . " and " - " symbols.
[a-z\.] - Any characters from a to z (only lowercase) as well as the " . " symbol.

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
