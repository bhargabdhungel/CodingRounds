# Implement Prototype of a UDP Network Protocol

## Problem Statement

There is a 2D array of size `n*2`, requests. At time t = `requests[i][0]`, `requests[i][1]` packets are to be sent over the network. The network can hold at most `max_packets`in the pipeline. It delivers the data to the client at rate of `rate` packets per second, ie `rate` packets are removed from the queue and delivered to client every second.

If the number of packets exceeds `max_packets` at any time the packets remaining at the time are dropped.

Given the array `requests`, and integers, `max_packets`, and `rate`, find the total number of packets that are dropped.

## Input Format

First line of input contains 3 integers `n` `max_packets` and `rate`
Next `n` lines contain pair `[time,requests]`

## Output Format

Output a single integer, the total number of packets that are dropped.

## Constraints

- `1 <= n <= 3e5`
- `1 <= max_packets <= 1e9`
- `1 <= rate <= 1e9`
- `1 <= requests[i][0], requests[i][1] <= 1e9`
- `requests[i][0] are pairwise distinct`

## Sample Testcases

### Input 1

```
3 10 2
1 8
4 9
6 7
```

### Output 1

```
4
```

### Explanation 1

| Time | Packets Left | Packets Sent | Total Packets | Dropped | Delivered |
| ---- | ------------ | ------------ | ------------- | ------- | --------- |
| 1    | 0            | 8            | 8             |         | 2         |
| 2    | 6            |              | 6             |         | 2         |
| 3    | 4            |              | 4             |         | 2         |
| 4    | 2            | 9            | 11            | 1       | 2         |
| 5    | 8            |              | 8             |         | 2         |
| 6    | 6            | 7            | 13            | 3       | 2         |
| 7    | 8            |              | 8             |         | 2         |
| 8    | 6            |              | 6             |         | 2         |
| 9    | 4            |              | 4             |         | 2         |
| 10   | 2            |              | 2             |         | 2         |

The total number of packets dropped is 1 + 3 = 4
