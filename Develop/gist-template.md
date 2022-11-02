# Regex Tutorial

Regular expressions are patterns used to match character combinations in strings. In JavaScript, regular expressions are also objects. These patterns are used with the exec() and test() methods of RegExp, and with the match(), matchAll(), replace(), replaceAll(), search(), and split() methods of String. This chapter describes JavaScript regular expressions.

## Summary

In this tutorial we will be showing you how the Regex is used to match an email address:

```const rexEmail = /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/;```

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

- ```^The matches any string that starts with The```
- ```end$ matches a string that ends with end```
- ```^The end$ exact string match (starts and ends with The end)```
- ```roar matches any string that has the text roar in it```

### Quantifiers

- ```abc* matches a string that has ab followed by zero or more c```
- ```abc+ matches a string that has ab followed by one or more c```
- ```abc? matches a string that has ab followed by zero or one c```
- ```abc{2} matches a string that has ab followed by 2 c```
- ```abc{2,} matches a string that has ab followed by 2 or more c```
- ```abc{2,5} matches a string that has ab followed by 2 up to 5 c```
- ```a(bc)* matches a string that has a followed by zero or more copies of the sequence bc```
- ```a(bc){2,5} matches a string that has a followed by 2 up to 5 copies of the sequence bc```

### OR Operator

- ```a(b|c) matches a string that has a followed by b or c (and captures b or c)```
- ```a[bc] same as previous, but without capturing b or c```

### Character Classes

- ```\d matches a single character that is a digit```
- ```\w matches a word character (alphanumeric character plus underscore)```
- ```\s matches a whitespace character (includes tabs and line breaks)```
- ````. matches any character```
