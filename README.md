# JavaScript Loose Comparison Bug

This repository demonstrates a common JavaScript bug related to loose comparison (==) of null or undefined values with numbers.  Loose comparison can lead to unexpected behavior, especially when dealing with potentially null or undefined function arguments.

## The Bug

The `bug.js` file contains a function `foo` that adds two numbers.  However, it doesn't handle the case where one or both arguments are null.  Using loose comparison (`==`) to check for null would lead to incorrect results in some cases.

## The Solution

The `bugSolution.js` file provides a corrected version of the `foo` function. It uses strict equality (`===`) to explicitly check for null values before performing the addition, ensuring correct behavior for all input cases.

## How to Reproduce

1. Clone the repository.
2. Navigate to the directory in your terminal.
3. Run `node bug.js` to see the bug in action.
4. Run `node bugSolution.js` to see the corrected behavior.