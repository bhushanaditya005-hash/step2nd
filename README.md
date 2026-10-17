# Problem 4: Exam Score Band Counter

Counts how many values in a sorted array fall within the inclusive range `[low, high]`.

## Sample output

```text
6
0
```

## Approach

- `lowerBound` finds the first index whose score is greater than or equal to `low`.
- `upperBound` finds the first index whose score is strictly greater than `high`.
- Subtract the indices to count all scores in the band.

The strict comparison matters because duplicate scores can appear at either edge. The lower bound must include every `low`, and the upper bound must move past every `high`.

## Complexity

Let `n` be the number of scores.

- **Linear scan:** `O(n)` time and `O(1)` auxiliary space.
- **Binary-search solution:** `O(log n)` time per query and `O(1)` auxiliary space.
- The solution uses two binary searches, so it does not scan all scores.

## Compile and run

```bash
javac ExamScoreBandCounter.java
java ExamScoreBandCounter
```
