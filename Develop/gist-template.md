# Introduction to Regex

This tutorial will introduce you what you need to know about regular expressions or commonly known as regex! Let's start with the basic definition, regex is a sequence of characters that defines a search pattern that helps match, locate and search through text. Once you learn the new syntax you will be able to user regex in almost any programming language! Let's dive a bit deeper and learn some syntax!

## Summary
In this tutorial you will learn how to search threw documents by using patterns to locate text using the regex syntax.

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
 " . " : The period operator matches any single character, for example sle.h will return aisle, isle, and  hassle.

"\ followed by a single character" : The backslash operator matches special characters as a single character, \.css$ will return any string ending in .css.

" $ " : The dollar sign operator matches any string where the pattern occurs at the end of the string. Ex. /e$/ matches apple and snapple but not apples.

" ^ " : The upward arrow matches any string where the pattern happens at the start of the string. Ex. ^apple matches apples but not snapple. 

" [] " : The bracket operator matches any one character inside the brackets, for example [abc] will return and string that a 'a', 'b', or 'c' occurs.

" () " : The parenthesis are used to group expressions!

### Anchors

Anchors can be used to to match certain positions by matching before, after, and between characters rather than matching any characters at all. 

" ^ " : Matches the position before the first character, for example ^b to the string "ball" matches b, but ^a does not match the word ball at all. 

" $ " : Matches the position  the end of the string. Ex "/e$/ in the string "Mongoose" returns true because e matches the end of the string.
### Quantifiers

Quantifiers returns how many times a character, character class, or group must be present for a match to be found. 

" * "  : Matches zero or more.

" + " : Matches one or more.

" ? " : Matches zero or one.

" { n } " Matches the quantity of n. 

" { n ,} " Matches at least n times.

" { n,m }" Matches from n to m. 

### OR Operator

The | (OR) operator  to match characters or strings of either the left or right of the operator. For example, apple|dog find the sting including  apple or dog.

### Character Classes

The character class matches only one out of several characters, for example if you place [fms] "flat", "mat", and "sat" would be returned. 

### Flags
 
 There are 6 flags: 

" g " : Matches the pattern multiple times.

" i "  : Makes the search case insensitive.

" u " : Adds support for unicode. 

" m " : Adds the multi-line mode, where " ^ " and " $ " matches the start and end of the whole string.

" s " : Short for single line. It causes the " . " operator to also match new line characters.

### Grouping and Capturing

For grouping and capturing we use round brackets " () " so that we can group a specific part of a regular expression together. This allows us to apply a quantifier to the whole group or restrict alternations to part of the regex.

### Bracket Expressions

" [] " : The bracket operator matches any one character inside the brackets, for example [abc] will return and string that a 'a', 'b', or 'c' occurs. You can also use a hyphen to define a set and the upward arrow (^) called meta-character to negate what is between the brackets. 

### Greedy and Lazy Match

Greedy match means it will match the longest possible string.

Lazy match means it will match the shortest string possible. 

For example, the greedy h.+l matches "hell" in the string "hello" because it is the longest match but, the lazy h.+?l matches "hel" because it is the shortest match.

### Boundaries

Boundaries (\b) is a meta-character anchor similar to the dollar sign because neither of them consume characters and matches zero-length. Boundaries match a specific position. There are three different positions that qualify as a boundaries: before the first character in a string, after the last character of the string, and between two characters of a string. 

### Back-references

Back-references match the same text of characters as previously matched by a capturing group and not only in the result or in the replacement string, but also in the pattern itself.

### Look-ahead and Look-behind

Look-ahead and look-behind is a zero-length assertion. The look-ahead and look-behind match characters but then gives up the match only returning the result, match or no match. They do not consume characters of the string but only assert wether a match is possible. 

## Author

My name is David Herring and I am a full-stack web developer. You can find my GitHub at https://github.com/davidherring1998. 


## Resources: 
<!-- https://learn.microsoft.com/en-us/dotnet/standard/base-types/quantifiers-in-regular-expressions -->

<!-- https://www.regular-expressions.info/charclass.html -->

<!-- https://stackoverflow.com/ -->

<!-- https://javascript.info/regexp-introduction -->

<!-- https://www.rexegg.com/regex-capture.html -->