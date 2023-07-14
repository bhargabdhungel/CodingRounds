# Sneakers Shopping

## Problem Statement

Jordan goes to a shop to buy `N` shoes. After his purchase, the shopkeeper offers him a crazy refund on his bill.<br>The shopkeeper tells Jordan that he can select any of the `[N/2]` shoes and the shopkeeper will refund the sum of the square of the prices of those shoes.

Now, before buying the shoes, Jordan can perform an infinite number of the following operations:

- Select any pair of two shoes.

- Let's say their cost is `A` and `B`, respectively.

- Update the cost of the first shoe as (`A OR B`)

- Update the cost of the second shoe to (`A AND B`)

Now, Jordan wonders what is the maximum refund he can get if the number and cost of the shoes are already decided. Help Jordan get the maximum benefit of this craziness.

Since the answer can be too great, output the answer modulo `1e9 + 7`

## Input Format

- The first line contains an integer representing `N`, the number of shoes.

- The second line contains `N` integers denoting the cost of those `N` shoes.

## Output Format

In a single line, print the maximum refund Jordan can get.

## Constraints

- `1 < N < 1e5`

- `1 < Price[i] <= 1e9`

## Sample Testcases

### Input 1

```
5
3 6 7 5 3
```

### Output 1

```
98
```
