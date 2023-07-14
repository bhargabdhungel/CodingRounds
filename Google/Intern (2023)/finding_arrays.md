# Finding Arrays

## Problem Statement

Given an array `S` of `N` elements. We need to find the count of distinct arrays `A` of `N` elements that exists such that:

- `A[i] < A[i + 1]` for all `1 <= i <= N`.

- Sum of digits of `A[i]` is equal to `S[i]` for all `1 <= i <= N`.

- `1 <= A[i] <= 1000`

An array `A` is said to be different from array `B` if there exists an index `i` such that `A[i] != B[i]`.

Since the count can be very large. Output the answer modulo `1e9 + 7`.

**Note**: Consider 1-based indexing.<br>

## Input Format

- First line contains an integer T, denoting the number of test cases.

- For each test case:

  - First line contains an integer N.

  - Second line contains N space-separated integers, denoting array S.

## Output Format

For each test case, print the required answer in a new line.

## Sample Testcases

### Input 1

```
1
2
2 1
```

### Output 1

```
10
```

### Explanation 1

Given arrays are possible:

1 — [2, 10]

2 — [2, 100]

3 — [2, 1000]

4 — [11, 100]

5 — [11, 1000]

6 — [20, 100]

7 — [20, 1000]

8 — [101, 1000]

9 — [110, 1000]

10 — [200, 1000]

### Input 2

```
4
3
10 15 16
6
3 6 10 14 12 17
10
3 9 9 3 11 7 14 15 11 17
9
2 7 3 5 9 13 9 14 11
```

### Output 2

```
101776
142727553
303300404
19829619
```

### Input 3

```
4
3
8 7 12
10
7 6 7 8 11 13 15 13 9 16
7
9 3 5 11 12 9 14
10
2 6 8 4 5 8 7 12 14 1

```

### Output 3

```
30242
629663671
288757998
868587712
```
