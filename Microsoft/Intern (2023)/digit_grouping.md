# Digit Grouping

## Problem Statement

There is an array consisting of `N` two-digit numbers. A group of numbers can be chosen from the array if every pair of chosen numbers has at least one common digit. For example, numbers 25 and 56 can be chosen together as they have a common digit 5, but 11 and 22 cannot be chosen together.

What is the maximum number of array elements that can be chosen together?

## Input Format

Write a function:

    int solution(int numbers[], int N);

## Output Format

Function returns the maximum number of its elements that can be chosen.

## Constraints

- `1 <= N <= 1e5`

- `10 <= numbers[i] <= 99`

## Sample Testcases

### Input 1

```
numbers = [50, 30, 15, 51, 10, 20, 15]
```

### Output 1

```
5
```

### Explanation 1

Numbers `50, 15, 51, 10, and 15` can be chosen. All pairs of chosen numbers have at least one common digit. For example, pair `(50, 15)` has a common digit 5; `(10, 50)` - digit O; `(51, 1O)` - digit 1.

### Input 2

```
numbers = [11 , 33, 55]
```

### Output 2

```
1
```

### Explanation 2

No two numbers have a common digit.
