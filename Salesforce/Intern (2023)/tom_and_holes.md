# Tom and Holes

## Problem Statement

As you know Tom always wants to catch Jerry. This time he is planning to dig M holes on a straight track. Digging one unit deep hole take one unit of time. Since Tom is lazy cat, he asks N fellow cats for help. Tom assigns each N cats some consecutive holes to dig. Two cats will not dig same hole Tom is very keen in catching Jerry, so he wants to assign holes to each cat optimally such that total time required to dig holes is minimum. But since Tom is weak in mathematics, can you help him find minimum amount of time required to all holes if he assigns holes to cats optimally.

## Input Format

First line contains T: Number of testcases<br/>
For each test case:<br/>
first line denotes 2 integers N M: i.e. number of cats and number of holes<br/>
Next line contains M space generated integers denoting the depth of each hole.

## Output Format

For each test case, output on new line, minimum amount of time required to dig all holes.

## Constraints

1 <= T <= 10<br/>
1 <= N <= M <= 100000<br/>
1 <= depth of holes <= 10000

## Sample Testcases

### Input 1

```
1
3 10
5 3 20 16 18 1 10 10 9 8
```

### Output 1

```
37
```

### Explanation 1

Ideal distribution of holes for all cats are:

cat1 = (5, 3, 20), cat2 = (16, 18, 1), cat3 = (10, 10, 9, 8)

Note: Although below distribution of holes yields a maximum time of 34 which is lesser than answer, but since consecutive holes are not assigned to cats, below distribution is invalid.

cat1 = (20, 9, 3, 1) total time = 33<br/>
cat2 = (18, 10, 15) total time = 33<br/>
cat3 = (16, 10, 8) total time = 34

### Input 2

```
2
4 5
1 2 3 4 5
2 2
1 1
```

### Output 2

```
5
1
```
