# JavaScript Type Error: Handling Undefined and Null

This repository demonstrates a common JavaScript error and its solution.  The error occurs when attempting to access the 'length' property of a variable that might be 'undefined' in addition to 'null'.

## The Bug

The `foo` function attempts to get the length of an array. It correctly handles the case where the input is `null`, returning 0. However, if the input is `undefined`, it throws a `TypeError` because `undefined` does not have a `length` property.

## The Solution

The solution involves explicitly checking for both `null` and `undefined` before accessing the `length` property.  This ensures that the function will not throw an error in these cases.