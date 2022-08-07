# Regex Tutorial

Tutorial explaining specific regex in regards to their definitions.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

The two anchor characters are ^ and $. The ^ anchor signifies a string that starts with the ^ and includes anything that follows it. It is important to not that regex is case sensitive and the first charcter with the ^ anchor will need to be an exact match. The $ is the end anchor signifying the string that is before it.

### Quantifiers

Quantifiers set the minimum and maximum limits of a regex string. There are a couple characters that signify different things for a quantifier.
* *—Matches the pattern zero or more times
* +—Matches the pattern one or more times
* ?—Matches the pattern zero or one time
* {}—Curly brackets can provide three different ways to set limits for a match:
  1. { n }—Matches the pattern exactly n number of times
  2. { n, }—Matches the pattern at least n number of times
  3. { n, x }—Matches the pattern from a minimum of n number of times to a maximum of x number of times

### OR Operator

The | OR operator breaks the requirements of a string pattern making grouping of charcters in a regex string writable in more than one way.

### Character Classes

A character class gives a difinition to a set of characters that occur in an input string. Some common character classes are:
* .—Matches any character except the newline character (\n)
* \d—Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].
* \w—Matches any alphanumeric character from the basic Latin alphabet, including the underscore (_). This class is equivalent to the bracket expression [A-Za-z0-9_].
* \s—Matches a single whitespace character, including tabs and line breaks

### Flags

Flags are placed after the second slash at the end of a regex and they help to define any additional information about the regex. The three most common flags are: 
* g—Global search: the regex should be tested against all possible matches in a string.
* i—Case-insensitive search: case should be ignored while attempting a match in a string
* m—Multi-line search: a multi-line input string should be treated as multiple lines

### Grouping and Capturing

Capturing groups takes the characters that match and squences them for possible re-use, while non-capturing groups do not. To make a grouping construct non-capturing we ad the characters ?: at the start of the expresssion being made inside parentheses.

### Bracket Expressions

A bracket expression is a range of numbers inside square brackets [] that we want to match and include. A hyphen - can be added to represent a range of possible characters.

### Greedy and Lazy Match

The term greedy means that the component will match as many occureneces of the patterns as possible. add the ? symbol after a component will make it lazy, making it match with as few patterns as possible.

### Boundaries

A boundary is placed before or after a set or sting to match with a particular word.

### Back-references

Back-reference expressions find the match and refers to the previous part of the expression. They are specidied with a backslash \ followed by a single digit.

### Look-ahead and Look-behind

The lookaround assertions look for wether or not there is a match or not and only returns with the result of "match" or "no match"

## Author

Miranda Mello
