# Secure Network

## Problem Statement

A secure communication network has been compromised and the cyber security team must restore its security. The network, `series`, is represented as a series of nodes identified using lowercase English letters. The nodes must be disconnected in order to remove the threat. In a single operation, any number of adjacent nodes identified by the same character can be disconnected. Find the minimum number of operations required to disconnect all the nodes and secure the network.

## Input Format

**string series**: a series of nodes

## Output Format

**int**: the minimum number of operations required to delete the entire series

## Constraints

- `1 <= series <= 500`
- `It is guaranteed that series contains lowercase English letters only.`

## Sample Testcases

### Input 1

```
aabbaa
```

### Output 1

```
2
```

### Explanation 1

aabbaa &xrarr; aaaa &xrarr; empty

The minimum number of operations required to delete the entire series is 2.

### Input 2

```
abaca
```

### Output 2

```
3
```

### Explanation 2

It is optimal to delete the substrings "b" and "c" first in two operations to get the string "aaa" which can be deleted in the next operation.

### Input 3

```
abcddcba
```

### Output 3

```
4
```

### Explanation 3

It is optimal to delete "dd" first to get "abccba". Then delete "cc" to leave "abba", "bb" to get "aa" and finally delete "aa".
