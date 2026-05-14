# Find the Kth Smallest Element of an Array

## Problem Statement

Given an array `arr[]` and an integer `k`, find the `kth` smallest element in the array.

---

## Approach

1. Sort the array using `Arrays.sort()`.
2. Return the element at index `k - 1`.

Since array indexing starts from `0`:

- 1st smallest element → index `0`
- 2nd smallest element → index `1`
- kth smallest element → index `k - 1`

---

## Java Code

```java
import java.util.Arrays;

class Solution {
    public int kthSmallest(int[] arr, int k) {

        Arrays.sort(arr);

        return arr[k - 1];
    }
}
```

---

## Example

### Input

```text
arr = [7, 10, 4, 3, 20, 15]
k = 3
```

### Sorted Array

```text
[3, 4, 7, 10, 15, 20]
```

### Output

```text
7
```

---

## Time Complexity

```text
O(n log n)
```

---

## Space Complexity

```text
O(log n)
```

---

## Concepts Used

- Arrays
- Sorting
- Indexing

---

## Problem Link

https://www.geeksforgeeks.org/problems/kth-smallest-element5635/1
