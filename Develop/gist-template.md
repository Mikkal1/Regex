# REGEX CRASH-COARSE-BOOTCAMP-TUTORIAL


## BRIEF INTRODUCTION TO REGEX

Regex or Regualar Expression is a computer coding tool. Regex is a specific order of charactars the provide a specific search instructions to computer. An example of a specific search would be for a computer to scan a body of text and capture all numerical charactars of that text such as a telephone number.

## Summary

This Crash Coarse Regex Tutorial will explore the Regex for Telephone numbers.
The following is Regex -  ^\d{3}-\d{3}-\d{4}$  The regular expression would be used to specically search for north american format telephone numbers.This Regex instructs the computer to search specially for 3 sets of numbers first a set of 3 numerical digits anywhere from 0 to 9 followed by a dash then another set of 3 numberical digits again, anywhere from zero to nine followed by a dash and finally a set of 4 nmerical digits anywhere ranging from 0-9. This is a search regex for a phone number of the following format xxx-xxx-xxxx.


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

    Anchors in Regex are basically the start and end point of the search string. The start of a regular expression is indicated with a Caret(^) and the einding indicater is the dollar sign ($). In between these two indicaters is where the specific search string should be. For example, using our telephone Regex search string, the exression would look like this ^\d{3}-\d{3}-\d{4}$ . With the Caret (^) at the begginning and the ($) at the end of the expression.


### Quantifiers

Regex quantifiers are the symbols or construct that define the quantity or repitition of a procedding character. For a telephone number we can use a contruct such as "\d{3}" . Between the double quotes is a Regex quantifier to search for a set of 3 numerical digits anywhere between 0-9.

### Grouping Constructs

Grouping Constructs with regular expressin is the ability to group charactars together and treat them as one unit. It can be done using parenthesis, where as anything within the parentesis can be considered part of one unit. For example a Regex with (416) would see these three numerical digits as one unit and search for this specific sequence.

### Bracket Expressions

In regular expressions, bracket expressions are used to define a set or range of characters that can match a single character at a specific position in the input text. They are enclosed within square brackets [ ]. For example [a-z] would match any lower case alpha character from a to z.
[0-9] this would capture any matching numerical character from 0-9.



### Character Classes

 In regular expressions character classes provide a way to match a single character out of a set or range of characters. They are defined within square brackets [ ] and allow you to specify which characters are acceptable at a particular position in the input text.For example [aeiou] is a contruct to search for all vowels.

### The OR Operator

The OR Operator can be used with the "|" symbol. it is used a logic OR. Meaning that there is a match as long as the alternative are present. For example. "Hot|Cold". There is a match considered as long as either Hot or Cold is entered as the input.




### Flags

Flags are modifiers in regular expressions, that are added to the pattern to change the behavior of the matching process. For example "/example/i
" the "i" after example will modify a expression to search for both lower and upper case characters.

### Character Escapes

In regular expressions Charactar Escapes are sequences of characters that have a special meaning and are used to represent specific characters or character classes. These escape sequences are preceded by a backslash \. Character escapes are employed to match characters that would otherwise be interpreted as special characters in the regular expression syntax.

### Throrough Breakdown Of This Tutorials Example Of a REGEX Search String For A Standard Phone Number.

"^\d{3}": This part specifies that the match must start with exactly three digits.

"^"     : Asserts the start of the string.

"\d{3}" : Matches exactly three digits.

"-"     : This is a literal hyphen that must be present in the string.

"\d{3}" : This part specifies that there must be exactly three digits after the hyphen.

"\d{3}" : Matches exactly three digits.

"-"     : Another literal hyphen.

"\d{4}$": This part specifies that the match must end with exactly four digits.

"\d{4}" : Matches exactly four digits.

"$"     : Asserts the end of the string.



## Author


Michael Ramcharitar Computer Coding Practitioner https://gist.github.com/Mikkal1/576734a1aca734cec7cb19c37cc0f302

conclusion:
Regular expressions are a great tool for text manipulation. Understanding the basics and practicing regularly will help you become proficient.
Remember that different programming languages may have variations in regex syntax, so be sure to check the documentation for the language you're working with.