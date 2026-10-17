# Problem 6: Class Attendance Tracker

This Java program counts the number of days a student was present and finds the longest consecutive streak of attendance.

## Sample 1

Input:
```text
[1, 1, 0, 1, 1, 1, 0, 1]
```

Output:
```text
Present: 6, Longest streak: 3
```

## Sample 2

Input:
```text
[0, 0, 0]
```

Output:
```text
Present: 0, Longest streak: 0
```

## Complexity

- **Time:** `O(n)`, because the array is traversed once.
- **Auxiliary space:** `O(1)`, because only a fixed number of variables are used.
- **Single pass:** Yes. Both the number of present days and the longest streak are calculated in the same loop.

## Compile and run

```bash
javac ClassAttendanceTracker.java
java ClassAttendanceTracker
```
