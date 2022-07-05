# Challenge-Module17-BC
Computer Science for JavaScript Challenge: Regex Tutorial


# Regex Tutorial on Matching an Email

Regular expressions can be used to find certain patterns of characters within a string. You can also find and replace a character or sequence of characters within a string. They are also frequently used to validate input. This regex matches character information for valid e-mail addresses.

## Summary

This is the regex code that we will be anaylizing today is: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Control characters]  character
- [Escape Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [ Greedy and Non-Greedy Match](#greedy-and- non-greedy-match)

## Regular expression atoms

### Anchors
- ^ matches at the beginning of the target string
- $ matches at the end of the target string

### Quantifiers
 - *   representing 0 or more occurrences of the atom,
 - +   representing 1 or more occurrence of the atom,
 - ?   representing 0 or 1 occurrences of the atom,
 - the bound {n}   representing exactly n occurrences of the atom,
 - the bound {m,n}   representing between m and n occurrences of the atom.

When we used `+` to communicate there is another sequence to be matched as a greedy quantifier. For Example `{n,m}` or `{3,9} as another greedy quantifer to specify the input should be a minimum of 2 characrtors to a maximum of 9 characters.

### Control characters

A backslash, \, followed by one of the characters a, b, f, n, r, t, v represents the ANSI-C interpretation of the control character

### Character Classes

In this Regex, the charactor class `/d` is used which in Javasctipt classifies the use of any digit from 0 to 9.

### Grouping and Capturing

There are 3 groups being captured in this example. The charactor class `/d` in 1st Group is the username of the email account `[A-Za-z0-9_\.-]` ~ "GistGit22". The 2nd group captures the domain name or e-mail service being used `[\da-z\.-]` ~"@.github" Lastly, the 3rd group captures the domain extention (i.e .com or .net) `[a-z\.]{2,6}`

### Bracket Expressions

Similar to groups in this example, there are also 3 bracket expressions. The information in the bracket expressions is opened and closed between brackets like this `[]`. This indentifies which information is allowed to be matched.

Bracket Expression first: `[A-Za-z0-9_\.-]` - includes non-case sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens.

Bracket Expression second: `[\da-z\.-]`   - includes all digits, case sensitive characters from a-z, periods and hyphens

Bracket Expression third: `[a-z\.]`      - includes case sensitive characters from a-z and periods.


### Greedy and Non-Greedy Match

Here, we have only used greedy quantifiers `+` and `{}`, meaning that it will allow the match to expand as long as it neess to go. If these quantifiers were non-greedy quantifiers, they would appear as `+?` or `{}?`, this will direct the system to make the shortest match.

## Author

MCX

### Repo

Here is my github repository: https://github.com/Mcnoor

### email

maxanoor@gmail.com
