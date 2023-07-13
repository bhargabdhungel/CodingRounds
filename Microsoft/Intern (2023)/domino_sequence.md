# Domino Sequence

## Problem Statement

A domino is a rectangular tile divided into two square parts. There are between 1 and 6 dots on each of the parts.

There is an array A of length `2 × N`, representing `N` dominoes. Dominoes are arranged in a line in the order in which they appear in array `A`. The number of dots on the left and the right parts of the `K-th` domino are `A[2K]` and `A[2K+1]` respectively. For example, an array `A = [2, 4, 1, 3, 4, 6, 2, 4, 1, 6]` represents a sequence of five domino tiles: `(2, 4), (1, 3), (4, 6), (2, 4), and (1, 6)`.

In a correct domino sequence, each pair of neighboring tiles should have the same number of dots on their adjacent parts. For example, tiles `(2, 4)` and `(4, 6)` form a correct domino sequence and tiles `(2, 4)` and `(1, 3)` do not.

What is the minimum number of domino tiles that must be removed from the sequence so that the remaining tiles form a correct domino sequence? It is **not allowed** to reorder or rotate the dominoes.

## Input Format

Write a function:

    int solution(vector<int> &A);

Array `A` represents a sequence of `N` domino tiles.

## Output Format

Function returns the minimum number of tiles that must be removed so that the remaining tiles form a correct domino.

## Constraints

- `1 <= N <= 50000`

- `length of array A = 2 × N`

- `1 <= A[i] <= 6`

## Sample Testcases

### Input 1

```
A = [2, 4, 1, 3, 4, 6, 2, 4, 1, 6]
```

### Output 1

```
3
```

### Explanation 1

The second and the last two dominoes should be removed. After this, the remaining dominoes are `(2, 4)` and `(4, 6)`.

### Input 2

```
A = [5, 1, 2, 6, 6, 1, 3, 1, 4 3, 4, 3, 4, 6, 1, 2, 4, 1, 6, 2]
```

### Output 2

```
7
```

### Explanation 2

The domino tiles that should remain are: `(2, 6)`, `(6, 1)`, `(1 , 2)`.

### Input 3

```
A = [1, 5, 3, 3, 1, 3]
```

### Output 3

```
2
```

### Explanation 3

No pair of dominoes can be connected without rotating or reordering them.

### Input 4

```
A = [3, 4]
```

### Output 4

```
0
```
