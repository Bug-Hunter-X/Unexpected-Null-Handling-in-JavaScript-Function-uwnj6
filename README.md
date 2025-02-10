# JavaScript Bug: Unexpected Null Handling

This repository demonstrates a common, yet subtle, bug in JavaScript related to null value handling. The `foo` function attempts to handle null inputs, but might not be completely robust in real-world scenarios.

## Bug Description

The `foo` function correctly handles explicit null inputs, returning 0. However,  it doesn't account for situations where either `a` or `b` might be implicitly null or undefined due to other parts of the code. This might lead to unexpected behavior or errors.

## Solution

The solution improves the null check to be more comprehensive using optional chaining and nullish coalescing.