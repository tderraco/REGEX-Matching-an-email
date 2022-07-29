# REGEX-Matching-an-email

Regex is a series of characters used to specify a search pattern in text. Regex is short for Regular Expression and can be used in a variety of different ways. 

## Summary

In this tutorial I will go over the how this Regex:

 `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

is used to validate if the string matches an email address
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

### Anchors
Anchors used in this Regex are `^` and `$`
The `^` indicates what needs to be at the begining of a string.
The `$` indicates that the antecedent code must be at the end of the string.
### Quantifiers
There are two quantifiers used in the regex which are `+` and `{2,6}`.
`+` is used to connect the Grouping Constructs (email name, the email service provider, and the .com.)
The `{2,6}`gives a range of 2-6 characters to match `[a-z\.]`.

### Grouping Constructs
There are 3 Grouping Constructs in this regex. Each construct will capture its respective matching data.
`([a-z0-9_\.-])`indicates the name of the email.
`([\da-z\.-])`indicates the email provider.
`([a-z\.]{2,6})` indicates the domain.



### Bracket Expressions
Bracket Expressions indicate a list of characters to match within the brackets. For an example `[a-z0-9_\.-]` will be looking to match any letter a-z, any number 0-9, and characters _,\,.,- .
`[\da-z\.-]` \d matches any single digit 0-9, a-z any letter from a-z, and characters _,\,.,-.
`[a-z\.]{2,6}` will match any letter a-z a minimum of 2 times but no more than 6.
### Character Classes
With character classes you single out certain characters within a bracket to match in a regex. In the above regex `a-z`will match any characters a-z and `0-9` any character 0-9.
### The OR Operator
There are no OR operators in this regex
### Flags
There are no flags in this expression
### Character Escapes
Character escapes matches characters with a special meaning. In this regex the `\`before a character will match whatever character that follows it.
## Author

Tracy Derraco
https://github.com/tderraco

