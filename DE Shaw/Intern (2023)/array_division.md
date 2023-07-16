# Array Division

## Problem Statement

An array `arr` is to be divided into multiple non-empty subarrays such that the total sum of costs of division is minimized. Each element of the array `arr[i]` is associated with a cost `cost[i]`.

The subarrays after division are numbered `1` to `m` where `m` is the number of subarrays. For example, if `arr = [1, 2, 3, 4]` is divided into two subarrays `[1, 2]` and `[3, 4]`, the subarray `[1, 2]` is numbered `1` and `[3, 4]` is numbered `2`.

The cost of a subarray starting from index `i` and ending at index `j` is defined as the product of value $$(arr[0] + arr[1] +...+arr[j]) + (k \cdot subarray \_ number)$$ and the sum of cost of the subarray i.e. $$(cost[i] + cost[i+1] + ... + cost[j]).$$ Thus the<br>cost of subarray from index `i` to `j` is $$(arr[0] + ... + arr[j] + k \cdot subarray \_ number) \times (cost[i] + ... + cost[j]).$$<br>Here `k` is the subarray number factor incurred in cost.

Given `arr`, cost of `n` integers each and the subarray number factor `k` incurred in cost, find the minimum total cost of the subarrays after optimal division.

## Input Format

Complete the function `getMinCost`:

`getMinCost` takes the following arguments:

- `int arr[n]`: the input array

- `int cost[n]`: the cost of elements

- `int k`: the subarray number factor incurred in cost

## Output Format

`long int`: the minimum cost of dividing the array

## Constraints

- `1 <= n <= 2000`

- `1 <= arr[i] <= 1000`

- `1 <= cost[i] <= 1000`

- `1 <= k <= 1000`

## Sample Testcases

### Input 1

```
n = 4
arr = [1, 2, 2, 1]
cost = [1, 3, 2, 1]
k = 0
```

### Output 1

```
26
```

### Explanation 1

It is optimal to divide the array into four subarrays `[1]`, `[2]`, `[2]` and `[1]`. The total cost thus will be $$((1 + 0 \cdot 1) \cdot 1) + ((1 + 2 + 0 \cdot 2) \cdot 3) + ((1 + 2 + 2 + 0 \cdot 3) \cdot 2) + ((1 + 2 + 2 + 1 + 0 \cdot 3) \cdot 1)$$

### Input 2

```
n = 3
arr = [3, 1, 4]
cost = [2, 3, 3]
k = 1
```

### Output 2

```
55
```
