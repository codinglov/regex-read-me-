# Title (replace with your title)

Regex is a short word for regular expressions.Regular expressions are a terms used by the computer to help people understand computer language.

## Summary

We are going to explore regex in javascript. Regex is a way to match certain expressions in a string. We are going to see how to code and implement Regex in the code and check it.

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

Regex has the following Components.
        -characters 
        -expressions
        -anchors
        -quantifiers



### Anchors

These special sequences match an empty substring.

    ^ matches at the beginning of the target string
    $ matches at the end of the target string
    \b matches on a word boundary, i.e., the previous or subsequent character is not a word character

### Quantifiers

These are used to generate unending matching possibilities. one of these quantifiers can be used:

    *   representing 0 or more occurrences of the match,
    +   representing 1 or more occurrence of the match,
    ?   representing 0 or 1 occurrences of the match,
    the bound {a}   representing exactly a occurrences of the match,
    the bound {a,b}   representing between a and b occurrences of the match. 
    ? used to indicate minimal/non-greedy/reluctant match . The default is always maximum
### Grouping Constructs

These describe the subexpressions of a regular expression and capture the substring og an input.

### Bracket Expressions

A bracket expression represents a character set through a list of characters enclosed by the square brackets: '[' and ']'. It normally matches the target string with any single character from the list.

If the character list begins with '^', it matches any single character not from the rest of the list.
If two characters in the list are separated by '???', this is shorthand for the (inclusive) range of characters between those two. It is illegal for two ranges to share an endpoint, e.g. a-c-e. Ranges are collating-sequence dependent and should be avoided for portability.

Most special characters lose their special status and become literals within brackets. Additionally,

    ??? is literal at the end or beginning of a bracket expression
    ^ is literal if not at the beginning of a bracket expression

### Character Classes

These define characters which can occur in an input string for successful match.

examples include:

A single character with no special significance represents that character in the target string. The characters with special significance (i.e. operator characters) are these:

    ^ . [ $ ( ) | * + ? { \

A non-alphanumeric character acts as the literal character (whether special or not) by escaping it, namely, adding \ in front of it.
Wild card. The . (period) special character matches any single character except \n (newline).

A backslash,\, followed by one of the characters 
a, b, f, n, r, t, v 
represents the ANSI-C interpretation of the control character

### The OR Operator

These are used to apply alternation to a chosen part of the string. it can be enclosed in parentheses,brackets . These character,.,looks like this ,|,


### Flags

Java Regex has a 6 flags in total each serving a different purpose.
    -i Ignores Casing therefore making expression search case-insensitively.
    -g Global which makes the expression search for all occurrence.
    -s DotAll makes ,., match new lines as well.
    -m Multiline makes the boundary characters ^ and $ match the beginning and ending of a string.
    -y Sticky makes expression start search from index indicated in lastIndex property.
    -u Unicode makes the expression assume individual characters as code points,not code units and thus match 32-bit characteras well.

### Character Escapes

These are special sequences representing commonly used character sets:

    \w is word (program identifier) character: [A-Za-z0-9_]
    \W is non-word character: [^A-Za-z0-9_]
    \s is a whitespace character: [ \f\n\r\t]
    \S is a non-whitespace character: [^ \f\n\r\t]
    \d is a digit character: [0-9]
    \D is a non-digit character: [^0-9]


## Credits

1. https://www.cs.wcupa.edu/rkline/index/regular-expressions.html
2. https://www.codeguage.com/courses/regexp/flags
3. http://www.microsoft.com/regex/mdocs 

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
