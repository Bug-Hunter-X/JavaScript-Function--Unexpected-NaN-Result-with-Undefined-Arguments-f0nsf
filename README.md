# JavaScript Function: Unexpected NaN Result with Undefined Arguments

This repository demonstrates a common JavaScript error related to handling undefined values in function arguments. The `foo` function attempts to handle null values but fails to account for undefined arguments, leading to NaN (Not a Number) results.

## Bug Description
The `foo` function correctly handles null values. However, if undefined values are passed as arguments, the addition operation results in NaN because undefined + number is NaN.

## Bug Solution
The solution involves explicitly checking for both null and undefined values using the loose equality operator (==) or the strict equality operator (===) to ensure that NaN results are prevented.  The solution also includes a clear error handling approach to notify the user if unexpected arguments are provided.

## How to reproduce the bug
1. Clone this repository.
2. Open `bug.js`.
3. Run the code using Node.js (node bug.js) or your preferred JavaScript environment.
4. Observe the output, noting the NaN result when undefined arguments are used.

## How to solve the bug
1. Replace `bug.js` with `bugSolution.js`.
2. Run the corrected code using Node.js (node bugSolution.js) or your preferred JavaScript environment.
3. Observe the output, noting the corrected handling of null and undefined arguments.