# The Finals
## Problem Statement
In the finals of the shooting competition, the last two participants going for the gold are James and Bob. Here are the rules of competition -
1. The two shooters would take turns to shoot
2. They shoot a row of markers (say `R` markers) which are `even` in number to make it fair to the two participants.
3. Each marker has a value written on it. Value is say `Ni` where `i` is the marker index
4. They can shoot at the end markers only & not in the middle. Else they would be disqualified.
5. The winner is the one with the maximum number of points at the end.

James has won the toss and will shoot first. As always, he is confused on the order to shoot in. Your goal is to help James win the event by guiding him through the order of markers to hit & hence, determine the maximum number of points he can win.

## Input Format
First line is the number of markers `R`.
Next `R` lines contain a marker of value of `Ni` where `i` lies within `[0,R-1]`.
## Output Format
Number indicating the maximum number of points
## Constraints
- `1 <= R <= 100`
- `1 <= Ni <= 1000`
## Sample Testcases

### Input 1
```
4
20
2
10
11
```
### Output 1
```
30
```
### Explanation 1
There are 4 markers 20 2 10 & 11 in order. James shoots 20 first. That leaves 2 10 11. Bob then shoots 11. James takes 10 and finally Bob takes 2. You helped James get 30 points & left Bob with 13 points only. Winner is James !!

### Input 2
```
4
11
20
2
10
```
### Output 2
```
30
```
### Explanation 2
Same numbers as previous example but a different order this time. Here you advise James to shoot 10 and not 11 even through the latter is the higher value. Bob takes 11 or could choose 2 for some reason. Remember only end markers. Both ways that allows James to take 20. And finally, marker 2 for Bob. so, you help James get 30 points and Bob gets 13 points. James is the winner.
If you had chosen 11 say for James at the beginning , Bob would have sho 20 and that leaves 10 for James & 2 for Bob. Bob would win with 22 points leaving James with 21 points.