# Special Subsequence

## Problem Statement

A subsequence of a string is a new string that is formed by deleting some (or none) of the characters from the original string, without changing the order of the remaining characters.

A special subsequence of a string is a subsequence that has the following properties:

- It has a length of exactly `K`.

- It contains all unique characters.

- The sum of the frequencies of all the characters in the subsequence is the maximum possible sum among all special subsequences of length `K`.

Given a string `S` and an integer `K`. find the number of distinct special subsequences of the string. Since the number of special subsequences can be large, print the answer modulo `1e9 + 7`.

## Input Format

- The first line contains an integer `T`, denoting number of test cases.

- For each test case:

  - First line contains an integer `N`

  - Second line contains an integer `K`

  - Next line contain a string `S`

## Output Format

For each test case, print the required answer in a new line.

## Constraints

- `1 <= T <= 10`

- `1 <= N <= 1e5`

- `1 <= K <= N`

- `S` contains only latin lowercase alphabets

## Sample Testcases

### Input 1

```
1
5
4
cppbg
```

### Output 1

```
2
```

### Explanation 1

2 subsequence are possible answer `cpbg` (includes p at index 1) and `cpbg` (includes p at index 2). Note: Consider 0 based indexing

### Input 2

```
1
12
8
fpbavjsmppdt
```

### Output 2

```
108
```

### Input 3

```
1
16
7
ppzfsncqyzmuwrcv
```

### Output 3

```
1680
```
