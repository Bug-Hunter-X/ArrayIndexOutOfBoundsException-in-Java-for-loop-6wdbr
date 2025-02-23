# ArrayIndexOutOfBoundsException in Java

This repository demonstrates a common Java programming error that leads to an `ArrayIndexOutOfBoundsException`. The error occurs when trying to access an array element using an index that is outside the valid range of indices (0 to array.length - 1).

## The Bug
The `bug.java` file contains the problematic code.  The for loop's condition `i <= arr.length` causes the loop to iterate one time more than it should. The last iteration attempts to access `arr[5]`, but the array only has indices from 0 to 4. This results in an `ArrayIndexOutOfBoundsException`.

## The Solution
The `bugSolution.java` file provides a corrected version of the code. The loop condition is changed to `i < arr.length`, ensuring that the loop terminates before attempting to access an invalid index.