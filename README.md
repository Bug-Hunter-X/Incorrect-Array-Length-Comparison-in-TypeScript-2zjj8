# TypeScript Array Comparison Bug

This repository demonstrates a subtle bug in a TypeScript function designed to compare two arrays for equality. The function incorrectly handles arrays of different lengths, returning `true` even when the arrays are of unequal length if the shorter array's elements match the beginning portion of the longer array.

## Bug Description
The `compareArrays` function fails to accurately compare arrays of differing lengths. It only checks elements up to the length of the shorter array. This results in unexpected behavior and incorrect comparisons.

## How to Reproduce
Clone this repository and run the TypeScript code.  Observe the incorrect output for the comparison of arrays with differing lengths.

## Solution
The solution involves correctly handling cases where the arrays have different lengths, ensuring that the function accurately reflects array inequality in these scenarios.  The corrected function is provided in `bugSolution.ts`.

## Lessons Learned
This bug highlights the importance of thorough testing and careful consideration of edge cases when writing comparison functions.  Always consider scenarios where input arrays might have different lengths, and explicitly handle these cases.