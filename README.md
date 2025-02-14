# MongoDB $inc Operator with Non-Numeric Value

This repository demonstrates an example of an uncommon error related to the MongoDB `$inc` operator. The `$inc` operator is used to increment a numeric field in a document.  Attempting to use it with a non-numeric value will result in an error.

## Bug
The bug lies in the incorrect usage of the `$inc` operator.  The code attempts to increment the `field` by the string 'abc', which is not a valid operation.

## Solution
The solution involves ensuring that the value being incremented is a number.  The updated code uses a numeric value for incrementing the field.

## How to reproduce the bug
1. Create a MongoDB collection
2. Insert a document with a numeric field
3. Run the code in `bug.js`
4. Observe the error