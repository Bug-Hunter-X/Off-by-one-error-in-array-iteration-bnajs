# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over arrays. The error occurs when the loop counter exceeds the valid index range of the array, leading to an `ArrayIndexOutOfBoundsException`.

## Bug Description

The provided Java code initializes an integer array of size 5 and attempts to populate it with even numbers. However, the `for` loop iterates from 0 up to `arr.length` (which is 5), causing an attempt to access `arr[5]`, which is beyond the valid index range (0-4). This results in an `ArrayIndexOutOfBoundsException`.

## Solution

The solution involves adjusting the loop condition to iterate from 0 up to `arr.length - 1`, ensuring that only valid array indices are accessed.