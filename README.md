# Off-by-One Error in Array Loop

This repository demonstrates a common off-by-one error in Java when iterating through an array. The error occurs in the for loop, which attempts to access an index beyond the array's bounds. 

## Bug Description
The code includes an error that causes an ArrayIndexOutOfBoundsException. The loop condition `i <= arr.length` should be changed to `i < arr.length`. The program attempts to access `arr[5]` while the array only has five elements (indexed 0-4). 

## Solution
The provided solution file corrects this by fixing the loop condition to `i < arr.length`. This prevents accessing elements beyond the allocated space in the array, effectively preventing the exception.

## How to reproduce the bug
1. Compile the `bug.java` file.
2. Run the compiled code. Observe the `ArrayIndexOutOfBoundsException`. 

## How to fix the bug
1. Replace the `bug.java` with `bugSolution.java`
2. Compile and run the code. The exception should no longer occur. 