# Unexpected Behavior of Loose Comparison with null in Javascript
This repository demonstrates an unexpected behavior in Javascript when using loose comparison (==) with null and numbers.  The issue stems from Javascript's type coercion during loose comparisons.

## Bug Description
The function `foo` intends to check if a number is null, negative, or positive. However, due to loose comparison, the result for `foo(0)` is incorrect, returning 1 instead of 0.

## Solution
The solution involves using strict comparison (===) to prevent type coercion and ensure accurate comparisons.