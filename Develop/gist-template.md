# REGEX Sample

When setting up a form to create or login to a form using an email regex is a standard way for the submissions to be verified if they are in the in the correct format. This is shorter and arguably more efficient way to search and format code to your specification. 

## Summary

This should give insight on how to setup a regex expression to verify if an email meets the required parameters.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Back-references](#back-references)

## Regex Components
(![Email verification Function with REGEX](images/function%20snip.png))
- this regular expression matches email addresses in the format username@domainname.tld
### Anchors
- The ^ anchor signifies a string that begins with the characters that follow it
- $ matches the end of the string

### Quantifiers
- {}—Curly brackets can provide three different ways to set limits for a match:
    { 2, 6 }—Matches the pattern from a minimum of 2 number of times to a maximum of 6 number of times
- +—Matches the pattern one or more times

### Character Classes
- .—Matches any character except the newline character (\n)
- \d—Matches any Arabic numeral digit and is equivalent to the bracket expression [0-9]

### Grouping and Capturing
- ([a-z0-9_\.-]+) matches one or more characters that are lowercase letters, numbers, underscores, dots, or hyphens, and captures them as a group representing the username portion of the email address
- @ matches the @ symbol
-([\da-z\.-]+) matches one or more characters that are digits, lowercase letters, dots, or hyphens, and captures them as a group representing the domain name portion of the email address
- \. matches a literal dot (.) character
- ([a-z\.]{2,6}) matches two to six characters that are lowercase letters or dots, and captures them as a group representing the top-level domain (TLD) portion of the email address

### Bracket Expressions
- Anything inside a set of square brackets ([]) represents a range of characters that we want to match
- They are also known as a positive character group, because they outline the characters we want to include
- [a-z]—The string can contain any lowercase letter between a–z
- [0-9]—The string can contain any number between 0–9
- [_.-]—The string can contain an underscore, hyphen, or period

### Back-references
href[https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial] 

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
