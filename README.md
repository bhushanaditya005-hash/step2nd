# Problem 7: Second-Best Score

Find the second-highest **distinct** score in an array without sorting it. Return `-1` if no second-highest distinct score exists.

## Sample output

```text
78
-1
```

## Approach

Track two values while visiting each score once:

- `highest`: the highest score seen so far.
- `second`: the second-highest distinct score seen so far.

If a score is greater than `highest`, move the old `highest` to `second`. Otherwise, update `second` only if the score is less than `highest` and greater than `second`. This skips duplicates of the highest score.

## Complexity

Let `n` be the number of scores.

- **One-pass solution:** `O(n)` time and `O(1)` auxiliary space.
- **Sorting first:** typically `O(n log n)` time, plus the space required by the sorting approach. Sorting is unnecessary here because two variables are enough.

## Compile and run

```bash
javac SecondBestScore.java
java SecondBestScore
```
