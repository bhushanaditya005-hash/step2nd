# Problem 8: Duty Roster Rotation

This Java solution rotates a roster to the right by `k` positions. Names that pass the end wrap around to the beginning.

## Sample output

```text
[D, E, A, B, C]
[D, E, A, B, C]
```

The second example uses `k = 7`. Since there are 5 names, `7 % 5 = 2`, so the result is the same as rotating right by 2 positions.

## Complexity

- **Time:** `O(n)`, because each name is moved once.
- **Auxiliary space:** `O(n)`, because a new array stores the rotated roster.
- **Why not rotate one place at a time?** Repeating a one-place rotation `k` times can take `O(n * k)` time. When `k` is very large, this does unnecessary work. Using `k % n` reduces the shift to fewer than `n` positions.

## Compile and run

```bash
javac DutyRosterRotation.java
java DutyRosterRotation
```
