# Regex Tutorial: Matching Email Addresses

Regex, short for regular expression, is essentially a sequence of characters that defines a specific search pattern. In code or search algorithms, regular expressions are used to find particular patterns of characters within a string. Regex can be utilized for replacing specific characters or sequences within a string and are also commonly used to validate input. This is a valuable asset when we encounter extensive code bases.

## Summary
As we have observed above, regex entails multiple purposes in programming and data manipulation. Regular expressions are instrumental in working with email addresses. When applied to email addresses, regex allows us to validate and extract email-related information from a given string. 

In other words, regex vastly enhances our ability to work with email addresses, as it provides both flexibility and accuracy in processing and validating email addresses. 

For this tutorial, we will be breaking down each section of the regex and covering what each character indicates. Below is the regex for email addresses:


`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`


## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Escaped Characters](#escaped-characters)
- [Conclusion](#conclusion)
- [Author](#author)

## Regex Components

### Anchors
Anchors play a vital role in regular expressions, as they serve as markers for the beginning and end of a string. In our email address regex, the caret symbol `(^)` signifies the *start* of the string, while the dollar symbol `($)` represents the *end*. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

By marking these anchors, we can verify that the returned search results will match the specific string pattern we defined.

### Quantifiers
Quantifiers, as the name suggests, determines the *limit* for strings. It can be either for the entire string or specific sections. 

In the email regex, the quantifier is applied to the *last* character of the string:  

`([a-z.]{2,6})` 

This indicates that the final part of an email address must consist of 2-6 characters.

### Character Classes
Character classes define sets of characters that are going to be matched within a string. 

In the email address regex pattern, there are a few character classes employed:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

One example is `\d`, which represents the digital character class, or the range 0-9. 

### Grouping and Capturing
A group in regex refers to a set of regex patterns that will be matched as a *unit* in your string. 

These groups can be identified by enclosing them within parentheses 
`(())`. 
### Bracket Expressions
Bracket expressions in regex are used to define a set of characters that will be matched *against* a string. These expressions are enclosed within square brackets `([])`, allowing you to specify a range or list of characters to be considered for a match.

### Escaped Characters
The`(\)`backslash is a character escape. This means that this character should *not* be denoted literally. In the email regex:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
1. `[a-z0-9_\.-]` 
We are not interpreting the `\` and looking for either `.` or `-` after the character escape. 
2. `[a-z\.]`
Similarly to the first example, we are ignoring the `\` and looking for `.`.


### Conclusion 
In conclusion, regex is an important concept for various reasons. In regards to this tutorial, regex helps us better understand how email addresses are interpreted and validated as a reliable form of communication. 
## Author

I am an aspiring web developer interested in becoming well-versed in full-stack development. If you wish to contact me, you can reach me at: 

Email: ima2132@columbia.edu 

GitHub: github.com/ima2132 