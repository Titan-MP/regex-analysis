# Regex-Analysis

Here we are doing an analysis of regular expression (Regex), and their functions and uses. We will be using the following regex to analyze and explain the different components of a regex.
## Summary

Here we will de discussing the different components of a regex, and how they are used. We will be using the following regex to analyze and explain the different components of a regex. These include Anchors, 
Quantofiers, OR Operator, Character Classes, Flags, Grouping and Capturing, Bracket Expressions, Greedy and Lazy Match, Boundaries, Back-references, Look-ahead and Look-behind.


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
A regular expression (shortened as regex or regexp; sometimes referred to as rational expression) is a sequence of characters that specifies a match pattern in text. Usually such patterns are used by string-searching algorithms for "find" or "find and replace" operations on strings, or for input validation.

/.+@.+\..+/

### Anchors

 \G This will match only at the starting point of the search or the position the previous successful match ended. Useful with the /g flag, or when you are only trying to match after a certain point in a string.
 Example: /\Gcat/gi will match only the first cat in the string "cat cat cat cat cat".
 Other examples of anchors are ^ and $.


### Quantifiers
Quantifiers are used to specify how many times a character, group, or character class must be present in the input for a match to be found. Quantifiers can be used with any character, group, or character class.

Examples of quantifiers are:
 + This will match the preceding token one or more times. For example, /a+/ will match the a in "candy" and all the a's in "caaaaaaandy".
 * This will match the preceding token zero or more times. For example, /bo*/ will match the 'boooo' in "A ghost booooed" and all the 'b' in "A bird warbled" while matching nothing in "A goat grunted".
 ? This will match the preceding token zero or one time. For example, /e?le?/ will match the 'el' in "angel" and the 'le' in "angle."
 {n} This will match the preceding token exactly n times. For example, /a{2}/ doesn't match the 'a' in "candy," but it matches all of them in "caandy," and the first two a's in "caaandy."
 {n,} This will match the preceding token n or more times. For example, /a{2,}/ doesn't match the 'a' in "candy," but matches all of them in "caandy" and in "caaaaaaandy."
 {n,m} This will match the preceding token at least n times, but no more than m times. For example, /a{1,3}/ will match nothing in "cndy", the 'a' in "candy," the two 'a's in "caandy," and the first three 'a's in "caaaaaaandy." Notice that when matching "caaaaaaandy", the match is "aaa", even though the original string had more a's in it.


### OR Operator
The | character is used to find a match for any one of the patterns separated by | as in: cat|dog|fish. For example, /green|red/ matches 'green' in "green apple" and 'red' in "red apple."

### Character Classes
Character classes are used to match the characters of a string. For example, the character class [abc] will match any of the characters a, b, or c; this is the same as [a-c], which uses a range to express the same set of characters. If you wanted to match only lowercase letters, your character class would be [a-z]. You can also include character ranges within a character class. For example, [a-zA-Z] matches all lowercase and uppercase letters.

### Flags
flags are used to perform case-insensitive and global searches. These flags can be used in any order, and are as follows:
g This flag is used to perform a global match (find all matches rather than stopping after the first match).
i This flag is used to ignore case.
m This flag is used to perform multiline matching.
u This flag is used to enable Unicode support. Used together with the "u" flag, the "y" flag prevents matches that start at or end at a previous match's ending position.
y This flag is used to perform "sticky" searches that match starting at the current position in the target string. See sticky for more information.

### Grouping and Capturing
Grouping and capturing are used to match multiple characters. To match a pattern multiple times, you need to use parentheses. For example, /(foo)/ matches and remembers "foo" in "foo bar." The matched substring can be recalled from the resulting array's elements [1], ..., [n] or from the predefined RegExp object's properties $1, ..., $9.


### Bracket Expressions
Bracket expressions are used to match one character from a certain set of characters. For example, the pattern [abc] will only match a single a, b, or c letter and nothing else. You can also specify a range of characters using the hyphen character. For example, [a-z] specifies a lowercase ASCII letter. To match a literal ] character, you need to escape it with a backslash, or place it as the first character in the list. For example, [()[\]{}] will match any of the literal characters '(', ')', '[', ']', '{', or '}'.

### Greedy and Lazy Match
Greedy and lazy quantifiers are used to match a string that has been repeated over and over again. Greedy quantifiers will match as many characters as possible, while lazy quantifiers will match as few characters as possible. For example, the greedy quantifier /a+/ applied to the string "baaaa" will match the entire string, while the lazy quantifier /a+?/ will only match the first 'a'.

### Boundaries
Boundaries are used to match a character that is not included in the character set. For example, the pattern \B../ will match any two characters that are not preceded by a word boundary. The pattern \B../ will match any two characters that are not followed by a word boundary.

### Back-references
A backreference is a way to match the same text as previously matched by a capturing group. Capturing groups count from 1, so the first capturing group's result can be referenced with \1 , the second with \2 , and so on. \0 is a character escape for the NUL character.

### Look-ahead and Look-behind
Look-ahead and look-behind are used to match text that is followed or preceded by other text. For example, the pattern (?=foo) will match any text that is followed by the text "foo". The pattern (?<=foo) will match any text that is preceded by the text "foo".
## Author
About the Author 
My name is Marc Rhymaun I am currently a student at UCF enrolled in the Coding Bootcamp. I am a full time student and work full time as well. I am currently working on a project that will help me and my team at work. I am looking forward to learning more about coding and how to apply it to my everyday life.
[GitHub](https://github.com/Titan-MP)
