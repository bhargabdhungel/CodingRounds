# Prime Path

## Problem Statement

Given `N X N` grid `G` and each cell of the grid contains an integer.

In one step you can move from cell `(i1,j1) to (i2,j2)` if `abs(i1-i2) + abs(j1-j2) <= p` at cost `floor( G[i1,j1]`^1/2^ `)`

Here `p` is the number of unique prime factors of `G[i1,j1]`.

Find the minimum cost to reach from `(1,1)` to `(N,N)`.

**Notes**:
- Use 1-based indexing.
- abs(x) denotes the absolute value of x or |x|.
- floor(x) denotes the largest integer less than or equal to x.

## Input Format

- The first line contains an integer `T`, denoting the number of test cases.

- For each test case:

  - The first line contains an integer `N` representing the size of the grid.
  - The next `N` lines contain `N` space-separated integers representing the grid.

## Output Format

For each test case, print the minimum cost to reach from `(1,1)` to `(N,N)` for each test case in a new line.

## Constraints

- `1 <= T <= 5`

- `1 <= N <= 1e3`

- `2 <= Gij <= 1e6`

- `1 <= i <= N`

- `1 <= j <= N`

## Sample Testcases

### Input 1

```
2
3
13 12 15
5 6 9
2 4 8
3 
2 3 5
30 4 6
5 2 8
```

### Output 1

```
7
5
```

### Explanation 1
- For the first test case:
- `N = 3` and `G` is given as:

| 13 | 12 | 15 |
|----|----|----|
| 5  | 6  | 9  |
| 2  | 4  | 8  |

- You can follow these steps
  - You can move from `(1,1)` to `(2,1)` at cost `floor(13`^1/2^`) = 3` since `(2-1)+(1-1) <= 1` and the number of unique prime factors of `13` is `1`.
  - You can move from `(2,1)` to `(2,2)` at cost `floor(5`^1/2^`) = 2` since `(2-2)+(2-1) <= 1` and the number of unique prime factors of `5` is `1`.
  - You can move from `(2,2)` to `(3,3)` at cost `floor(6`^1/2^`) = 2` since `(3-2)+(3-2) <= 2` and the number of unique prime factors of `6` is `2`.

- Thus to move from `(1,1)` to `(3,3)` the minimum cost is `3+2+2 = 7`.


### Input 2

```
2
3
18 3 4
6 5 9
13 20 14
3
18 10 20
14 2 5
14 19 10
```
### Output 2

```
9
7
```
### Input 3

```
2
3
14 20 4
19 12 5
20 15 12
3
3 6 3
6 18 18
4 15 9
```
### Output 3

```
6
6
```