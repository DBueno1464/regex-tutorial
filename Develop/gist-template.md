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

This is how the email regex looks like. 

```
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
```

Our regex has to be wrapped in forward slashes, '/'. Also, each component is put in parantheses,'()'. The brackets, '[]', will also be disussed later in [Bracket Expressions](#bracket-expressions).

If we loosely break up this regex:
- a-z: this string can contain lowercase letters from a to z.
- 0-9: this string can contain numbers from 0 to 9.
- _.-: this string can contain an underscore, period and a hyphen. (We exclude the backslash since its purpose is to allow the period (.) to be used as a parameter not as a meta character.)

followed by an @, then:
- \d: any digit character, including numbers from 0 to 9.
- a-z: this string can contain lowercase letters from a to z.
- .-: this string can contain a period and hyphen.

followed by a ., then:
- a-z: this string can contain lowercase letters from a to z.
- .: this string can contain a period.

### Anchors

The characters ^ and $ are considered anchors.

```
'^' signifies a string that begins with the characters that follow it. An example, "^pie" will find any words that contain the letters 'p', 'i', and 'e' in that order, like 'piece'. The anchor, ^, will find words that contain the characters that immediately follow it.
```

```
'$' signifies a string that ends with the characters that precede it. An example, "wed$" would find the word 'followed'.
```

### Quantifiers


### Grouping Constructs

### Bracket Expressions

Anything inside square brackets ([]) are characters we wish to match. All components in our regex are contained in distinct square brackets. These 'components' are called bracket expressions. Bracket expressions, in other words, outline the charactes we want to include in our search.

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
