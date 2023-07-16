# Hybrid Maximum

## Problem Statement

A hybrid sequence is a sequence that can be divided into two disjoint subsequences. Every Subsequence is an array.

Given two arrays `A` and `B` of sizes `N` and `M` respectively. You are also given a hybrid sequence `S`.

The expression $\sum_{i=1}^{N+M} \max(S_1,\ldots, S_i) - \sum_{i=1}^{N+M} \max(S_1,\ldots, S_i)$ calculates the difference between the sum of the maximum values and the sum of the minimum values in the hybrid sequence `S`.

Find the maximum value of the expression for all possible hybrid sequences `S`.


**Note**:
- Use 1-based indexing.
- A subsequence is a sequence obtained by deleting zero or more numbers (not necessarily consecutive ) from the original sequence and maintaining the relative order of the remaining numbers.

## Input Format

- The first line contains an integer `T`, denoting the number of test cases.

- For each test case:

  - The first line contains an integer `N` denoting the number of elements in array `A`.
  - The second line contains `N` space-separated integers denoting the elements of array `A`.
  - The third line contains an integer `M` denoting the number of elements in array `B`.
  - The fourth line contains `M` space-separated integers denoting the elements of array `B`.

## Output Format

For each test case, print the maximum value of the expression in a new line.

## Constraints
- `1 <= T <= 1000`
- `1 <= N, M <= 1000`
- `1 <= A[i] <= 1e6`
- `1 <= B[i] <= 1e6`
- `sum of N x M over all test cases <= 1e7`

## Sample Testcases

### Input 1

```
1
3
1 2 3
2
4 1
```

### Output 1

```
12
```

### Explanation 1
The hybrid sequence `S = [1 4 1 2 3]` gives the maximum value of the expression.

$\left(\sum_{i=1}^{N+M} \max(S_1,\ldots, S_i)\right) = 1 + 4 + 4 + 4 + 4 = 17$
$\left(\sum_{i=1}^{N+M} \min(S_1,\ldots, S_i)\right) = 1 + 1 + 1 + 1 + 1 = 5$
$\left(\sum_{i=1}^{N+M} \max(S_1,\ldots, S_i)\right) - \left(\sum_{i=1}^{N+M} \min(S_1,\ldots, S_i)\right) = 17 - 5 = 12$
### Input 2

```
1
2
5 1
2
5 3
```

### Output 2

```
12
```

### Input 3

```
1
2
1 5
2
3 5
```

### Output 3

```
12
```