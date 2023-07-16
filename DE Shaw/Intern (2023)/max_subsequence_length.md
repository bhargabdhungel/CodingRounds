# Maximum Subsequence Length

## Problem Statement

Given an array `arr` of `n` integers, the indexed weighted sum of a subsequence of the array formed by choosing the indices $$[i_1, i_2, ..., i_k]$$ is defined as $$(i_1 \cdot k + a[i_1]) + (i_2 \cdot k + a[i_2]) + ... + (i_k \cdot k + a[i_k])$$ assuming indexing starts from 1, where k is the length of subsequence. For example, for the array `arr = [1, 10, 100]`, the indexed weighted sum of the subsequence formed by the indices `[1, 3]` is $$(1 \cdot 2 + 1) + (3 \cdot 2 + 100) = 3 + 106 = 109$$.

Given `arr` and an integer `max_sum`, find the length of the longest subsequence with an indexed weighted sum less than of equal to `max_sum`.

## Input Format

Complete the function `getMaxSubsequenceLen`:

`getMaxSubsequenceLen` takes two parameters:

- `int arr[n]`: the input array

- `int max_sum`: the maximum allowed sum of the subsequence

## Output Format

`long int`: the maximum possible length of the subsequence

## Constraints

- `1 <= n <= 2 × 1e5`

- `1 <= arr[i] <= 1e4`

- `1 <= max_sum <= 1e15`

It is guaranteed that at least one of the elements of the `arr` is less than `max_sum`.

## Sample Testcases

### Input 1

```
n = 3
arr = [2, 3, 5]
max_sum = 11
```

### Output 1

```
2
```

### Explanation 1

The optimal subsequence is formed by indices `[1, 2]` i.e. `[2. 3]` with index weighted sum $$(1 \cdot 2 + 2) + (2 \cdot 2 + 3) = 4 + 7 = 11$$

### Input 2

```
n = 4
arr = [4, 3, 2, 1]
max_sum = 33
```

### Output 2

```
3
```
