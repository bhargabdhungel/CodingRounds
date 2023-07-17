# Special Subarrays

## Problem Statement

You are given an array `arr` of size `N` of non negative integers. Find number of subarrays of array which are special. A subarray is special if product of its maximum and minimum element in divisible by length of the subarray.

## Input Format

- The first line contains `T` denoting the number of test cases.

- For each test case:

  - The first line contains `N` denoting the size of the array.

  - The next line contains `N` space separated integers denoting the elements of the array.

## Output Format

For each test case, print the number of special subarrays.

## Constraints

- `1 <= T <= 1000`

- `1 <= N <= 10^5`

- `0 <= arr[i] <= 30`

## Sample Testcases

### Input 1

```
1
5
50 30 45 43 73
```

### Output 1

```
3
```
