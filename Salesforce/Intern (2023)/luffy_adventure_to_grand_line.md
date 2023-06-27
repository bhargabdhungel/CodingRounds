# Luffy adventure to Grand Line

## Problem Statement

One day, Luffy is on an adventure and came across a stone bridge that takes him to the grand line. The stone bridge has each stone labeled with a random String of characters S. Luffy has to cross the bridge by jumping only onto special characters else if he jumps on any other character he falls into the ocean.

Now make sure he steps on all stones labeled with special characters on the way. Obviously, he has to take multiple consecutive jumps throughout this path.

He is interested in finding out the maximum length of a single jump, he has to take to cross the stone bridge. Each character on the badge is at
a distance of 1. Formally consider that Luffy is at the start of the bridge. His goal is to reach the end of the bridge. In every jump, Luffy jumps anywhere on the next stone with a special character on the bridge. If Luffy cannot cross the bridge then return -1.

Note: All characters apart from [A..Z][a..z] are treated as special characters

## Constraints

Assume the length of S is n.

1 <= n <= 1e6

## Sample Testcases

### Input 1

```
ABK@2azxy@gk
```

### Output 1

```
5
```

### Input 2

```
ABCSD
```

### Output 2

```
-1
```
