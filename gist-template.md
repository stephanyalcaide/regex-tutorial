# Regex tutorial

Regex or regular expression that define a pattern 

## Summary

I will be give you an explanation of the following code works.
Code: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Conclusion](#conclusion)
## Regex Components

### Anchors
The Anchors that are used to maintain this regular expression are: "^" to start, and "$" to finish.
### Quantifiers
In this code, we are using "+" to show that there is another sequence to be paired as quantifier. We also used "{2,6}" as another greedy quantifier to specify the minimum of 2 characters or maximum of 6 characters.
### Grouping Constructs
There are three groups in this code. 
Group #1 is the username of the e-mail account "[a-z0-9_\.-]". 
The 2nd group gets the domain name or e-mail service being used 
"[\da-z\.-]". 
Finally, the 3rd group gets the domain (i.e .com or .net) "[a-z\.]{2,6}"
### Bracket Expressions
Kind of like the groups in this code, there are also 3 bracket expressions. The information in the bracket expressions are opened and closed brackets like this "[]". 

Bracket Expression #1: "[a-z0-9_\.-]" - includes sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens.

Bracket Expression #2: "[\da-z\.-]" - shows us all numbers, case sensitive characters from a-z, periods and hyphens

Bracket Expression #3: "[a-z\.]" - includes case sensitive characters from a-z and periods.
### Character Classes
Inside this regex, the character class "/d" Javascript classifies the use of any digit from 0 to 9.
### The OR Operator

### conclusion
Code: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
Our anchors indicate that we are starting at "^" and ending at "$", matching the entire string
The ? quantifier tells us that the "#" symbol is optional
The regex will match the string of characters grouped within the ()
Within "[]", we see that the characters will include the range of 0-9.
According to the quantifiers and the OR Operator {2,6} | it will be 2-6.
So, in conclusion, if your hex value in question is a single group of characters that may or may not begin with '#', contains 2,6 characters from the range of letters a-z and/or whole numbers 0-9.
### Author 
stephany alcaide
https://github.com/stephanyalcaide