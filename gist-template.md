# Regex Tutorial

Introductory paragraph (replace this with your text)

## Summary

A regex or also known as regular expression is a string of characters that helps define a specific search pattern. The one we will be using today is `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` which is used to match a hex value.

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
The characters `^`, `$`are anchors.  

- `^` is the beginning of a string or line
- `$` is the end of a string or line

#### Example
 In `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` the hex value would be `#?([a-f0-9]{6}|[a-f0-9]{3})`. The `^` and `$` can be seen at the beginning and end of the expression. 

### Quantifiers
Quantifiers specify how many characters or symbols is needed to be a match for an input. Most commonly used are `{n}` and `?`.

#### Example
`{n}` is used to match exactly *n* times. In our string `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` the `{n}` here would be `{6}` and `{3}`.

`?` is used to specify if it matches once or zero times. It is also used on the preceeding character which in the string `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` it is `#`.  

### Grouping Constructs

### Bracket Expressions
Bracket expressions use `[]` to specify what range of characters you want to match

#### Example
`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` in this string the `[]` are using a `-` or a hyphen. This hyphen is searching for lowercase letters a-f and numbers 0-9.

### Character Classes
Using lowercase and uppercase letters can let you mix and match digits and characters classes

#### Example
`/^?[a-f0-9]{6}/` This would be considered only lowercase 
`/^?[A-f0-9]{6}/` This would be considered matching since it has upper and lowercase. 

### The OR Operator
The OR operator uses `|` which lets you match one or more different patterns. 

#### Example 
In this string `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` the OR operator is in the middle of the two bracket expressions. So the OR operator would match either `[a-f0-9]{6}` and or `[a-f0-9]{3}`.

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
