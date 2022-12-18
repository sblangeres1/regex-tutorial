# Title (replace with your title)

Regex is what is known as regular text. Regex are used when developers need to define filters
for example on inputs like a login. Regex is basically characters that define a search pattern
in text.

## Summary
The goal of this tutorial is to explain the components
of a regex or a regular expression, used to match a hex value in HTML. A hex value is a color code with a value that informs the device as to how much of the color should appear on the screen. Here is an example snippet:
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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
`/^`#?([a-f0-9]{6}|[a-f0-9]{3})`$/`

Anchors are used at the start and end of a regex string expression and do not match any other characters in a regex. The anchors are highlighted in the snippet above.

### Quantifiers
/^#`?`([a-f0-9]`{6}`|[a-f0-9]`{3}`)$/

Quantifiers tell you how many characters are expected and it tells you how many specific characters have to be in the input for there to be a match. '?' tells us that this expression will match 0 or 1 time. In our snippet the quantifiers are `{6}` and `{3}`. Another example of this is: #FFFFFF and #FFF.

### OR Operator
/^#?([a-f0-9]{6}`|`[a-f0-9]{3})$/

The OR operator tells us that the component can match either string that is on either side of the `|`. Using our snippet, we are told that our hex value is either 6 or 3 characters.

### Character Classes
/^#?(`[a-f0-9]`{6}|`[a-f0-9]`{3})$/

Character Classes tell what kind of characters can be input and you put them in square brackets. With our example we should expect to see letters `a-f` and numbers `0-9`
 
### Flags

Flags are components that modify the default searching of a regex and they are optional. When it comes to flags there are only 6 of them. Flags appear as single lowercase letters. The 6 listed are: `i`, `g`, `s`, `m`, `m`, `y` and `u`. Our code snippet does not have any flags.

### Grouping and Capturing

Grouping is a useful way to group multiple regex patterns so we dont have to create a capture group. A capturing group gives extra information when we use a regular expression to match a string.

### Bracket Expressions
/^#?`([a-f0-9]{6}|[a-f0-9]{3})`$/

Bracket expressions tell us where the beginning of a character class or quantifier statement is. Brackets tell us that any character in them will match. With our example we use parenthesis to define our bracket expression.

### Greedy and Lazy Match
/^#`?`([a-f0-9]{6}|[a-f0-9]{3})$/

A greedy match matches elements as many times as it can be. A lazy match matches an element as little times as possible.

### Boundaries

Boundaries are `\b` or `\B`. `\b` represents an anchor which matches positions where one side is a word and the other is not a word. `\B` matches everything where \b doesn't.

### Back-references

Back-references match the text that capturing groups already matched. Using opening tag lets the user reuse the tag name for the closing tag. `\1` is often used for this.

### Look-ahead and Look-behind

Look-ahead shows what follows the current position in the string. Look-behind shows what is behind the current position in the string.

## Author

My name is Scottie Blangeres, I am a web development student currently learning at UC Davis Continued Education.
My GitHub is [sblangeres1](https://github.com/sblangeres1)
