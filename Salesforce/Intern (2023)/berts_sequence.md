# Bert's Sequence

## Problem Statement

Bert has a fascination for sequences, he found a very nice problem with natural number sequences.

He has a number n which indirectly implies that he has an integer sequence of [1, 2, 3, ..., n-1]. Now he asks Ernie to remove the minimum amount of elements from this sequence, such that the product of all integers in the resulting sequence becomes congruent to 1 mod n. [i.e., if the product of the resultant sequence is p, then p%n is 1]

Note:

1. For all practical purposes, consider the product of an empty sequence to be 1.

2. If there are multiple sequences, return the lexicographically smallest one.

3. Return the array in increasing order only.

## Input Format

An integer (n) will be given as the argument of the function that you need to complete.

## Output Format

Return an integer array of relevant size.

## Constraints

2 <= n <= 1e5

## Sample Testcases

### Input 1

```
7
```

### Output 1

```
1 2 3 4 5
```

### Explanation 1

The product of the elements is 120 which is congruent to 1 modulo 7. The only longer subsequence is [1, 2, 3, 4, 5, 6]. Its product is 720 which is congruent to 6 modulo 7. Hence the answer is [1, 2, 3, 4, 5].
