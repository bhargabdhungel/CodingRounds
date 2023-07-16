# Median Path

## Problem Statement

Given a tree of `n` nodes and `n-1` edges. Each node has a value, which is sorted in an arrya `C`. `Ci (1 <= i <= n)` denotes the value of node `i`.

Find the sum of the median values of all the simple paths of odd length starting from node `1`.

**Notes**:
- Use 1-based indexing.
- The median of an array is the middle element of a sorted array.
- A simple path is a path that does not contain any node more than once.
- A tree is a connected graph with no cycles.

## Input Format

- First line contains an integer `T`, denoting the number of test cases.

- For each test case:

  - The first line contains an integer `n` denoting the number of nodes in the tree.
  - The second line contains `n` space-separated integers denoting the values of the nodes.
  - The next `n-1` lines contain two space-separated integers `u` and `v` denoting an edge between nodes `u` and `v`.

## Output Format

For each test case, print the answer in a new line representing the sum of the median values of all the simple paths of odd length starting from node `1`.

## Constraints

- `1 <= T <= 10`

- `1 <= n <= 1e5`

- `1 <= Ci <= 1e9`

## Sample Testcases

### Input 1

```
1
5
7 6 9 10 1
1 2
2 3
1 4
2 5
6
1 2 4 3 1 5
1 4
4 3
1 2
2 5
2 6
```

### Output 1

```
20
7
```