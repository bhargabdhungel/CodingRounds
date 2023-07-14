# Minimize Operations

## Problem Statement

Consider a weighted tree with `N` nodes and `N-1` edges. You have the option to select an edge and adjust its weight by either increasing or decreasing it by 1 in a single operation.<br>There are `Q` queries given, each consisting of two nodes `U` and `V`. <br>Your task is to determine the minimum number of operations required to make the weight of every edge on the path from node `U` to node `V` equal.<br>Please note that if `U` and `V` are identical, no operations need to be performed.

You need to calculate the minimum number of operations needed to equalize the weight of each edge on the path from node U to node V for every query.

## Input Format

- The first line contains a single integer `N`.

- Next `N-1` lines contain 3 space-separated integers `U`, `V`, and `W` denoting an edge between the nodes `U` and `V` with weight `W`.

- The next line contains a single integer denoting `Q`.

- The next lines contain 2 space-separated integers `U`, `V` denoting the queried path.

## Output Format

Print a list of `Q` space-separated integers where the th integer denotes the answer to the ith query.

## Constraints

- `1 < N < 1000`

- `1 <= Edges[i][0] < N`

- `1 <= Edges[i][1] < N`

- `1 <= Edges[i][2] < 26`

- `1 < Q <= 1e5`

- `1 <= Queries[i][0] <= N`

- `1 < Queries[i][1] <= N`

## Sample Testcases

### Input 1

```
3
1 2 3
1 3 2
1
2 3
```

### Output 1

```
1
```

### Input 2

```
7
1 2 3
1 3 4
2 4 4
2 5 6
3 6 6
3 7 8
1
2 7
```

### Output 2

```
5
```
