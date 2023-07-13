# Anagram Sum

## Problem Statement

Joey had neatly arranged some words using plastic alphabets corresponding to the integers zero through nine. But as he went to show his project to his dad, he tripped and all his alphabets got jumbled up. Can you find the sum of all the words he had arranged, so he gets an A for effort?

## Input Format

The first line contains the jumbled string S. There can be multiple instances of each integer word in S. You can assume are no extra letters in the string.

## Output Format

An integer which has the sum of all integers in the jumbled string S.

## Constraints

- `1 <= S.length <= 5×10^5`

## Sample Testcases

### Input 1

```
ehfrzeevteeonoir
```

### Output 1

```
9
```

### Explanation 1

On unscrambling the input, we get: "zeroonethreefive" or 0135. The sum of all the integers is 9 (=0+1+3+5).
