# Problem 10: Busiest Bus Row

A Java solution that finds the row with the largest sum in a 2D grid. If multiple rows have the same sum, it returns the row with the smallest index.

## Example

Input:
```text
[[2, 0, 1],
 [3, 3, 1],
 [1, 1, 1]]
```

Output:
```text
Row 1, Total 7
```

## Complexity

- **Time:** `O(r * c)`, where `r` is the number of rows and `c` is the number of columns.
- **Auxiliary space:** `O(1)`; only a fixed number of variables are used. The returned two-element array is output space, also `O(1)`.

## Compile and run

```bash
javac BusiestBusRow.java
java BusiestBusRow
```
