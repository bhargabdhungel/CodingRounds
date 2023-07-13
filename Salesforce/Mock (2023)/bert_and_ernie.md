# Bert and Ernie

## Problem Statement

Bert and Ernie are bored and they want to play a game. They stumble into a lot of magical beans and each bean has a "special string" inside it. A special string is defined as a binary string that reads the same both ways. In other words, special strings have 2 properties:

1. It is made of only 0s and 1s.

2. It reads the same from both sides (left to right and right to left), for example, 1001 or 10101

Both players play on each special string by taking alternate turns with Ernie going first. In each turn, a player can perform one of the following actions:

1. Modify: Choose any index i, where s[i] = '0' and convert it to '1'. It costs 1 rupee.

2. Upside-Down: For 0 rupee, reverse the whole string. This action is only allowed if the string is currently not a "special string", and the last action was not Upside-Down, i.e., if Ernie uses this action on the string, then Bert can't use it in the next move, and vice versa.

The game, for a single "special string", will end when all the values in it become '1'.

Winner: If both of them play optimally, then whoever spends the least amount of money wins that game. If they spend an equal amount of money it is a TIE.

Note: Given that there are multiple magic beans, hence there will be multiple games played by Bert and Ernie. You have to find the result of all those games, more about this in the input/output section.

## Input Format

An array of strings will be given as input.

You need to complete the function in which the input described above will be passed as arguments (specialStrings array).

## Output Format

Return a string array in which the result of each game is present as per the problem statement. [Results can be BERT, ERNIE, TIE]

## Constraints

- `1 <= size of "array of special-strings" <= 10^4`
- `1 <= size of "special-strings" <= 10^5`
- `The Sum of the size of all "special strings" won't exceed 10^6 per test file.`

## Sample Testcases

### Input 1

```
2
1001
00111100
```

### Output 1

```
BERT
BERT
```

### Explanation 1

1. in the 1-st move, Ernie has to perform the 1-st action(Modify action) as the string is currently a "special string", [pays 1 rupee] (string becomes 1101)

2. in the 2-nd move, Bert reverses(Upside-Down action) the string. [pays 0 rupee] (string becomes 1011)
