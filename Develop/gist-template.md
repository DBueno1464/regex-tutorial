# Matching an Email

Regular expressions, or regex, are patterns used to find and match specific character combinations in strings or text. These expressions are very useful for when you want to find specific words in files of text. Regular expression can also be used to find ANY phone number, email, etc in text. They can do this by finding characters that follow a specific pattern that matches what you are looking for. In this tutorial, I will explain how regular expressions are created and how the are to be read and interpreted.

## Summary

The regex expression that I will be covering in this tutorial is the email regex. This regex finds any email in any form of text. As you may know, an email is split into three main components; the user's chosen name, the domain and the extension. 

```
flyingpanda@gmail.com
```
Here we can split up the email like so:
- flyingpanda
- gmail
- com

After splitting the email into these three components we can see that they respectively match the components stated above.

Note: In an email there will always be an '@' between the user's chosen name and the domain. Same can be said about a '.' between the domain and the extension.

This is how the email regex looks like.

```
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
```

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

### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
