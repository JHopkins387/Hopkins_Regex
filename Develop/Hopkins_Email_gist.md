# Hopkins' Regex Tutorial on Matching an Email

Regular expressions can be used to find certain patterns of characters within a string. You can also find and replace a character or sequence of characters within a string. They are also frequently used to validate input. This regex matches character information for valid e-mail addresses.

## Summary

We will be analyzing the piece of code; /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

Anchors are to contain the express, in this case it starts wit  a ^ and it ends with a $.
### Quantifiers

The example I have here is that we use the + to communicate that another sequence can be matched as a greedy quantifier.  ALso, we used the {2,6} as a Greedy quantifier to tell that the input should have a minimum of 2 characters used but a maximum of 6.

### Character Classes

This expression uses the character class of /d, which is used in Javascript to classify the use of digits that can go from 0 to 9.

### Grouping and Capturing

This example has 3 different groupings used.  The first group represents the email account "[a-z0-9\.-]". Group 2 is used to capture the email service or domain used "[\da-z\.-]".  The 3rd and final group represents the domain extension (.com, .org, .net) which is "[a-z\.]{2,6}"

### Bracket Expressions

Similar to the groups used in this example, there are three blanket expressions.  The information used in each bracket is contained in the [].  This lets us know which info is allowed to be matched.

Bracket Expression 1: [a-z0-9_\.-] : This includes the case sensitive characters ranging from a-z, as well as the numbers from 0-9, an underscore, periods, and hyphens.

Bracket Expression 2: [\da-z\.-] : This includes all digits, the case sensitive characters from a-z, the periods, and hyphens.

Bracket Expression 3: [a-z\.] : This includes the case sensitive characters from a-z and the periods.
### Greedy and Lazy Match

This example we only used greedy quantifiers `+` and `{}`, which meaning that it allows the match to expand as long as it needs to go for it to work. If the quantifiers that were used lazy quantifiers, they would have showed up as `+?` or `{}?`, this would direct the system to make the shortest match possible.

## Author

Hi I am Jarrett Hopkins, and coding is interesting to say the least.
Here is a link to my github repos: https://github.com/JHopkins387
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
