# Maximise Collection

## Problem Statement
Given `N` toys in a shop, each with a price represented by an array `A` of size `N`. You have a certain amount of money `C`, that you can spend on toys. There are also `K` toys that are broken and you don't want to buy them.

For each `Q` query, find the maximum number of toys you can buy with the given amount of money `C` while avoiding the broken toys.

**Note**:
- Use 1-based indexing.
- Query definition:
  - The first element of the query is the amount of money `C = Query[i][0]`
  - The second element of the query is the number of broken toys `K = Query[i][1]`
  - The next `K` integers represent the indices of the broken toys which are `Query[i][j]` for all `j >= 2`
  - Treat all the queries independently

## Input Format

- The first line contains an integer `T`, denoting the number of test cases.

- For each test case:
    - The first line contains an integer `N` denoting the number of toys in the shop.
    - The second line contains `N` space-separated integers denoting the prices of the toys.
    - The third line contains an integer `Q` denoting the number of queries.
    - The next `Q` lines:
        - The first element of the query is the amount of money `C`
        - The second element of the query is the number of broken toys `K`
        - The next `K` integers represent the indices of the broken toys.


## Output Format

For each test case, print `Q` space-separated integers denoting the maximum number of toys you can buy in a new line.

## Constraints

- `1 <= T <= 10`
- `1 <= N <= 1e5`
- ``1 <= A[i] <= 1e6`
- `1 <= Q <= 1e4`
- `1 <= C <= 1e9`
- `1 <= K <= 10`
- `1 <= Query[i][j] <= N for all j >= 2` 

## Sample Testcases

### Input 1

```
1
10
7 3 6 8 2 1 4 9 5 10
4
10 2 2 5
15 1 1
20 2 1 2 3
100 0
```

### Output 1

```
3 5 5 10
```

### Explanation 1

**query 1**:
- `C = 10`, `K = 2`, `broken = [2, 5]`
- You can buy toys `[6 7 9]` which cost a total of `A[6] + A[7] + A[9] = 1 + 4 + 5 = 10`
- You can buy at most `3` toys.

**query 4**:
- `C = 100`, `K = 0`, `broken = []`
- You can buy all the toys which cost a total of `55` amount of money.
- You can buy at most `10` toys.
